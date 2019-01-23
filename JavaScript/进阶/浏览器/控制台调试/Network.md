
# 1

[Chrome 开发者工具中文文档](http://www.css88.com/doc/chrome-devtools/network-performance/resource-loading/)

# 2

1.通过浏览器输入网址的行为，统一为“GET”方法；

2.GET提交的数据会在地址栏中显示出来，而POST提交，地址栏不会改变；

3.get是把参数数据队列加到提交表单的ACTION属性所指的URL中，值和表单内各个字段一一对应，在URL中可以看到。
post是通过HTTPpost机制，将表单内各个字段与其内容放置在HTML HEADER内一起传送到ACTION属性所指的URL地址。
用户看不到这个过程。

4.get传送的数据量较小，不能大于2KB。post传送的数据量较大，一般被默认为不受限制

5.[HTTP Request Header 请求头](https://blog.csdn.net/lipeigang1109/article/details/59057525)

6.[postman 使用post方式提交参数值](https://www.cnblogs.com/haoxuanchen2014/p/7771459.html)

7.[Cookie](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Cookies)

# 3
<article class="devsite-article-inner">  
  <h1 itemprop="name" class="devsite-page-title">
    了解 Resource Timing
  </h1>
<p>了解通过网络收集资源的阶段至关重要。这是解决加载问题的基础。</p>
<h3 class="hide-from-toc" id="tldr_hide-from-toc">TL;DR</h3>
<ul>
<li>了解 Resource Timing 的阶段。</li>
<li>了解每个阶段向 Resource Timing API 提供的内容。</li>
<li>了解时间线图表中不同的性能问题指示器，例如一系列透明栏或者大片的绿块。</li>
</ul>
<p>所有网络请求都被视为资源。通过网络对它们进行检索时，资源具有不同生命周期，以 Resource Timing 表示。Network 面板使用与应用开发者所用相同的 <a href="http://www.w3.org/TR/resource-timing">Resource Timing API</a>。</p>
<p>请Note: 当使用具有跨源资源的 Resource Timing API 时，确保所有资源具有 CORS 标头。</p>
<p>Resource Timing API 提供了与接收各个资源的时间有关的大量详细信息。请求生命周期的主要阶段包括：</p>
<ul>
<li>重定向</li>
<li>立即开始 <code>startTime</code>。</li>
<li>如果正在发生重定向，<code>redirectStart</code> 也会开始。</li>
<li>如果重定向在本阶段末发生，将采集 <code>redirectEnd</code>。</li>
<li>应用缓存</li>
<li>如果是应用缓存在实现请求，将采集 <code>fetchStart</code> 时间。</li>
<li>DNS</li>
<li><code>domainLookupStart</code> 时间在 DNS 请求开始时采集。</li>
<li><code>domainLookupEnd</code> 时间在 DNS 请求结束时采集。</li>
<li>TCP</li>
<li><code>connectStart</code> 在初始连接到服务器时采集。</li>
<li>如果正在使用 TLS 或 SSL，<code>secureConnectionStart</code> 将在握手（确保连接安全）开始时开始。</li>
<li><code>connectEnd</code> 将在到服务器的连接完成时采集。</li>
<li>请求</li>
<li><code>requestStart</code> 会在对某个资源的请求被发送到服务器后立即采集。</li>
<li>响应</li>
<li><code>responseStart</code> 是服务器初始响应请求的时间。</li>
<li><code>responseEnd</code> 是请求结束并且数据完成检索的时间。</li>
</ul>
<p><img alt="Resource Timing API 示意图" src="https://developers.google.cn/web/tools/chrome-devtools/network-performance/imgs/resource-timing-api.png"></p>
<h2 id="devtools" style=""><a href="#top_of_page" class="devsite-back-to-top-link material-icons" data-tooltip-align="b,c" data-tooltip="返回页首" aria-label="返回页首" data-title="返回页首"></a>在 DevTools 中查看</h2>
<p>要查看 Network 面板中给定条目完整的耗时信息，您有三种选择。</p>
<ol>
<li>将鼠标悬停到 Timeline 列下的耗时图表上。这将呈现一个显示完整耗时数据的弹出窗口。</li>
<li>点击任何条目并打开该条目的 Timing 标签。</li>
<li>使用 Resource Timing API 从 JavaScript 检索原始数据。</li>
</ol>
<p><img alt="Resource Timing 信息" src="https://developers.google.cn/web/tools/chrome-devtools/network-performance/imgs/resource-timing-data.png"></p>
<figure>
<figcaption>
<p>
  此代码可以在 DevTools 的 Console 中运行。
  它将使用 Network Timing API 检索所有资源。
  然后，它将通过查找是否存在名称中包含“style.css”的条目对条目进行过滤。
  如果找到，将返回相应条目。
</p>
<code>
  performance.getEntriesByType('resource').filter(item =&gt; item.name.includes("style.css"))</code>

</figcaption>
<img src="https://developers.google.cn/web/tools/chrome-devtools/network-performance/imgs/resource-timing-entry.png" alt="Resource Timing 条目">
</figure>

<dl>

  <dt class="queued"><strong>Queuing</strong></dt>
  <dd>
    如果某个请求正在排队，则指示：
      <ul>
        <li>
        请求已被渲染引擎推迟，因为该请求的优先级被视为低于关键资源（例如脚本/样式）的优先级。
        图像经常发生这种情况。        </li>
        <li>
        请求已被暂停，以等待将要释放的不可用 TCP 套接字。        </li>
        <li>
        请求已被暂停，因为在 HTTP 1 上，浏览器仅允许每个源拥有<a href="https://crbug.com/12066">六个 TCP 连接</a>。        </li>
        <li>
        生成磁盘缓存条目所用的时间（通常非常迅速）        </li>
      </ul>
  </dd>

  <dt class="stalled"><strong> Stalled/Blocking</strong></dt>
  <dd>
    请求等待发送所用的时间。
    可以是等待 Queueing 中介绍的任何一个原因。
    此外，此时间包含代理协商所用的任何时间。</dd>

  <dt class="proxy-negotiation"><strong> Proxy Negotiation</strong></dt>
  <dd>与代理服务器连接协商所用的时间。</dd>

  <dt class="dns-lookup"><strong><abbr data-tooltip-align="b,c" data-tooltip="Domain Name System" aria-label="Domain Name System" data-title="Domain Name System"> DNS</abbr> Lookup</strong></dt>
  <dd>
    执行 DNS 查询所用的时间。
    页面上的每一个新域都需要完整的往返才能执行 DNS 查询。</dd>

  <dt class="initial-connection"><strong> Initial Connection / Connecting</strong></dt>
  <dd>建立连接所用的时间，包括 <abbr data-tooltip-align="b,c" data-tooltip="Transmission Control Protocol" aria-label="Transmission Control Protocol" data-title="Transmission Control Protocol">TCP</abbr> 握手/重试和协商 <abbr data-tooltip-align="b,c" data-tooltip="Secure Sockets Layer" aria-label="Secure Sockets Layer" data-title="Secure Sockets Layer">SSL</abbr> 的时间。</dd>

  <dt class="ssl"><strong> SSL</strong></dt>
  <dd>完成 SSL 握手所用的时间。</dd>

  <dt class="request-sent"><strong> Request Sent / Sending</strong></dt>
  <dd>
    发出网络请求所用的时间。
    通常不到一毫秒。</dd>

  <dt class="ttfb"><strong> Waiting (<abbr data-tooltip-align="b,c" data-tooltip="Time To First Byte" aria-label="Time To First Byte" data-title="Time To First Byte">TTFB</abbr>)</strong></dt>
  <dd>
    等待初始响应所用的时间，也称为至第一字节的时间。
    此时间将捕捉到服务器往返的延迟时间，以及等待服务器传送响应所用的时间。</dd>

  <dt class="content-download"><strong> Content Download / Downloading</strong></dt>
  <dd>接收响应数据所用的时间。</dd>
</dl>

<h2 id="_1"><a href="#top_of_page" class="devsite-back-to-top-link material-icons" data-tooltip-align="b,c" data-tooltip="返回页首" aria-label="返回页首" data-title="返回页首"></a>诊断网络问题</h2>
<p>通过 Network 面板可以发现大量可能的问题。查找这些问题需要很好地了解客户端与服务器如何通信，以及协议施加的限制。</p>
<h3 id="_2">已被加入队列或已被停止的系列</h3>
<p>最常见问题是一系列已被加入队列或已被停止的条目。这表明正在从单个网域检索太多的资源。在 HTTP 1.0/1.1 连接上，Chrome 会将每个主机强制设置为最多六个 TCP 连接。如果您一次请求十二个条目，前六个将开始，而后六个将被加入队列。最初的一半完成后，队列中的第一个条目将开始其请求流程。</p>
<p><img alt="被停止的请求系列" src="https://developers.google.cn/web/tools/chrome-devtools/network-performance/imgs/stalled-request-series.png"></p>
<p>要为传统的 HTTP 1 流量解决此问题，您需要实现<a href="https://www.maxcdn.com/one/visual-glossary/domain-sharding-2/">域分片</a>。也就是在您的应用上设置多个子域，以便提供资源。然后，在子域之间平均分配正在提供的资源。</p>
<p>HTTP 1 连接的修复结果<strong>不会</strong>应用到 HTTP 2 连接上。事实上，前者的结果会影响后者。
如果您部署了 HTTP 2，请不要对您的资源进行域分片，因为它与 HTTP 2 的操作方式相反。在 HTTP 2 中，到服务器的单个 TCP 连接作为多路复用连接。这消除了 HTTP 1 中的六个连接限制，并且可以通过单个连接同时传输多个资源。</p>
<h3 id="_3">至第一字节的漫长时间</h3>
<p><small>又称：大片绿色</small></p>
<p><img alt="长 TTFB 指示灯" src="https://developers.google.cn/web/tools/chrome-devtools/network-performance/imgs/indicator-of-high-ttfb.png"></p>
<p>等待时间长表示至第一字节的时间 (TTFB) 漫长。建议将此值控制在 <a href="https://developers.google.cn/speed/docs/insights/Server">200 毫秒以下</a>。长 TTFB 会揭示两个主要问题之一。</p>
<p>请执行以下任一操作：</p>
<ol>
<li>客户端与服务器之间的网络条件较差，或者
2.服务器应用的响应慢</li>
</ol>
<p>要解决长 TTFB，首先请尽可能缩减网络。理想的情况是将应用托管在本地，然后查看 TTFB 是否仍然很长。如果仍然很长，则需要优化应用的响应速度。可以是优化数据库查询、为特定部分的内容实现缓存，或者修改您的网络服务器配置。很多原因都可能导致后端缓慢。您需要调查您的软件并找出未满足您的性能预算的内容。</p>
<p>如果本地托管后 TTFB 仍然漫长，那么问题出在您的客户端与服务器之间的网络上。很多事情都可以阻止网络遍历。客户端与服务器之间有许多点，每个点都有其自己的连接限制并可能引发问题。测试时间是否缩短的最简单方法是将您的应用置于其他主机上，并查看 TTFB 是否有所改善。</p>
<h3 id="_4">达到吞吐量能力</h3>
<p><small>又称：大片蓝色</small></p>
<p><img alt="吞吐量能力指示符" src="https://developers.google.cn/web/tools/chrome-devtools/network-performance/imgs/indicator-of-large-content.png"></p>
<p>如果您看到 Content Download 阶段花费了大量时间，则提高服务器响应或串联不会有任何帮助。首要的解决办法是减少发送的字节数。</p>

  </div>    

<p>Except as otherwise noted, the content of this page is licensed under the <a href="https://creativecommons.org/licenses/by/3.0/">Creative Commons Attribution 3.0 License</a>, and code samples are licensed under the <a href="https://www.apache.org/licenses/LICENSE-2.0">Apache 2.0 License</a>. For details, see our <a href="https://developers.google.cn/terms/site-policies">Site Policies</a>. Java is a registered trademark of Oracle and/or its affiliates.</p>
<p class="devsite-content-footer-date" itemprop="datePublished" content="2018-07-23T14:33:48.791310">   
      上次更新日期：七月 23, 2018
</p>



