<div class="article-intro" id="content">
<h2>Document 对象</h2>
<p>当浏览器载入 HTML 文档, 它就会成为 <strong>Document 对象</strong>。</p>
<p>Document 对象是 HTML 文档的根节点。</p>
<p>Document 对象使我们可以从脚本中对 HTML 页面中的所有元素进行访问。</p>
<p><b>提示：</b>Document 对象是 Window 对象的一部分，可通过 window.document 属性对其进行访问。</p>

<hr>
<h2>浏览器支持</h2>
<p>
<p>所有主要浏览器都支持 Document 对象。</p>

<hr>
<h2>Document 对象属性和方法</h2>
<p>HTML文档中可以使用以下属性和方法:</p>



<table class="reference notranslate">
<tbody><tr>
<th width="35%" align="left">属性 / 方法</th>
    <th align="left">描述</th>
</tr>
<tr>
    <td><a href="prop-document-activeelement.html">document.activeElement</a></td>
    <td>返回当前获取焦点元素</td>
</tr>
<tr>
    <td><a href="met-document-addeventlistener.html">document.addEventListener()</a></td>
    <td>向文档添加句柄</td>
</tr>

<tr>
<td><a href="/jsref/met-document-adoptnode.html" rel="noopener" target="_blank">document.adoptNode(node)</a></td>
	<td>从另外一个文档返回  adapded 节点到当前文档。</td>
</tr>
<tr>
<td><a href="coll-doc-anchors.html">document.anchors</a></td>
    <td>返回对文档中所有 Anchor 对象的引用。</td>
</tr>
<tr>
<td>document.applets</td>
    <td><p>返回对文档中所有 Applet 对象的引用。</p><p><span class="deprecated"><b>注意:</b> HTML5 已不支持 &lt;applet&gt; 元素。</span></p></td>
</tr>
<tr>
<td><a href="prop-doc-baseuri.html">document.baseURI</a></td>
	<td>返回文档的绝对基础 URI</td>
</tr>
<tr>
<td><a href="/jsref/prop-doc-body.html" rel="noopener" target="_blank">document.body</a></td>
    <td>返回文档的body元素</td>
</tr>
<tr>
<td><a href="met-doc-close.html">document.close()</a></td>
    <td>关闭用 document.open() 方法打开的输出流，并显示选定的数据。</td>
</tr>
<tr>
<td><a href="prop-doc-cookie.html">document.cookie</a></td>
    <td>设置或返回与当前文档有关的所有 cookie。</td>
</tr>
<tr>
<td><a href="met-document-createattribute.html">document.createAttribute()</a></td>
	<td>创建一个属性节点</td>
</tr>
<tr>
<td><a href="met-document-createcomment.html">document.createComment()</a></td>
	<td>createComment() 方法可创建注释节点。</td>
</tr>
<tr>
<td><a href="met-document-createdocumentfragment.html">document.createDocumentFragment()</a></td>
	<td>创建空的 DocumentFragment 对象，并返回此对象。</td>
</tr>
<tr>
<td><a href="met-document-createelement.html">document.createElement()</a></td>
	<td>创建元素节点。</td>
</tr>
<tr>
<td><a href="met-document-createtextnode.html">document.createTextNode()</a></td>
	<td>创建文本节点。</td>
</tr>
<tr>
<td><a href="prop-document-doctype.html">document.doctype</a></td>
	<td>返回与文档相关的文档类型声明 (DTD)。</td>
</tr>
<tr>
<td><a href="prop-document-documentelement.html">document.documentElement</a></td>
	<td>返回文档的根节点</td>
</tr>
<tr>
<td><a href="prop-doc-documentmode.html">document.documentMode</a></td>
    <td>返回用于通过浏览器渲染文档的模式</td>
</tr>
<tr>
<td><a href="prop-document-documenturi.html">document.documentURI</a></td>
	<td>设置或返回文档的位置</td>
</tr>
<tr>
<td><a href="prop-doc-domain.html">document.domain</a></td>
    <td>返回当前文档的域名。</td>
</tr>
<tr>
<td>document.domConfig</td>
	<td><span class="deprecated"><b>已废弃</b>。</span>返回 normalizeDocument() 被调用时所使用的配置。</td>
</tr>
<tr>
	<td><a href="/jsref/coll-doc-embeds.html" rel="noopener" target="_blank">document.embeds</a></td>
	<td>返回文档中所有嵌入的内容（embed）集合</td>
</tr>
<tr>
<td><a href="coll-doc-forms.html">document.forms</a></td>
    <td>返回对文档中所有 Form 对象引用。</td>
</tr>
<tr>
<td><a href="met-document-getelementsbyclassname.html">document.getElementsByClassName()</a></td>
	<td>返回文档中所有指定类名的元素集合，作为 NodeList 对象。</td>
</tr>
<tr>
<td><a href="met-document-getelementbyid.html">document.getElementById()</a></td>
	<td>返回对拥有指定 id 的第一个对象的引用。</td>
</tr>
<tr>
<td><a href="met-doc-getelementsbyname.html">document.getElementsByName()</a></td>
    <td>返回带有指定名称的对象集合。</td>
</tr>
<tr>
<td><a href="met-document-getelementsbytagname.html">document.getElementsByTagName()</a></td>
	<td>返回带有指定标签名的对象集合。</td>
</tr>
<tr>
<td><a href="coll-doc-images.html">document.images</a></td>
    <td>返回对文档中所有 Image 对象引用。</td>
</tr>
<tr>
<td><a href="prop-document-implementation.html">document.implementation</a></td>
	<td>返回处理该文档的 DOMImplementation 对象。</td>
</tr>
<tr>
<td><a href="met-document-importnode.html">document.importNode()</a></td>
	<td>把一个节点从另一个文档复制到该文档以便应用。</td>
</tr>
<tr>
<td><a href="prop-document-inputencoding.html">document.inputEncoding</a></td>
	<td>返回用于文档的编码方式（在解析时）。</td>
</tr>
<tr>
<td><a href="prop-doc-lastmodified.html">document.lastModified</a></td>
    <td>返回文档被最后修改的日期和时间。</td>
</tr>
<tr>
<td><a href="coll-doc-links.html">document.links</a></td>
    <td>返回对文档中所有 Area 和 Link 对象引用。</td>
</tr>
<tr>
<td><a href="met-document-normalize.html">document.normalize()</a></td>
	<td>删除空文本节点，并连接相邻节点</td>
</tr>
<tr>
<td><a href="met-document-normalizedocument.html">document.normalizeDocument()</a></td>
	<td>删除空文本节点，并连接相邻节点的</td>
</tr>
<tr>
<td><a href="met-doc-open.html">document.open()</a></td>
    <td>打开一个流，以收集来自任何 document.write() 或 document.writeln() 方法的输出。</td>
</tr>

<tr>
    <td><a href="met-document-queryselector.html">document.querySelector()</a></td>
    <td>返回文档中匹配指定的CSS选择器的第一元素</td>
</tr>
<tr>
<td><a href="/jsref/met-document-queryselectorall.html" rel="noopener" target="_blank">document.querySelectorAll()</a></td>
    <td>document.querySelectorAll() 是 HTML5中引入的新方法，返回文档中匹配的CSS选择器的所有元素节点列表</td>
</tr>
<tr>
<td><a href="prop-doc-readystate.html">document.readyState</a></td>
    <td>返回文档状态 (载入中……) </td>
</tr>
<tr>
<td><a href="prop-doc-referrer.html">document.referrer</a></td>
    <td>返回载入当前文档的文档的 URL。</td>
</tr>
<tr>
    <td><a href="met-document-removeeventlistener.html">document.removeEventListener()</a></td>
    <td>移除文档中的事件句柄(由 addEventListener() 方法添加)</td>
</tr>
<tr>
<td><a href="met-document-renamenode.html">document.renameNode()</a></td>
	<td>重命名元素或者属性节点。</td>
</tr>

<tr>
<td><a href="/jsref/coll-doc-scripts.html" rel="noopener" target="_blank">document.scripts</a></td>
	<td>返回页面中所有脚本的集合。</td>
</tr>
<tr>
<td><a href="prop-document-stricterrorchecking.html">document.strictErrorChecking</a></td>
	<td>设置或返回是否强制进行错误检查。</td>
</tr>
<tr>
<td><a href="prop-doc-title.html">document.title</a></td>
    <td>返回当前文档的标题。</td>
</tr>
<tr>
<td><a href="prop-doc-url.html">document.URL</a></td>
    <td>返回文档完整的URL</td>
</tr>
<tr>
<td><a href="met-doc-write.html">document.write()</a></td>
    <td>向文档写 HTML 表达式 或 JavaScript 代码。</td>
</tr>
<tr>
<td><a href="met-doc-writeln.html">document.writeln()</a></td>
    <td>等同于 write() 方法，不同的是在每个表达式之后写一个换行符。</td>
</tr>
</tbody></table>
<br><hr>
<h2>警告 !!!</h2>
<p>在 W3C DOM核心，文档对象
继承节点对象的所有属性和方法。</p>
<p>很多属性和方法在文档中是没有意义的。</p>
<p><strong>HTML 文档对象可以避免使用这些节点对象和属性：</strong></p>

<table class="reference notranslate">
<tbody><tr>
<th width="30%" align="left">&nbsp;属性 / 方法</th>
<th align="left">避免的原因</th>
</tr>
<tr>
<td>document.attributes</td>
	<td>文档没有该属性</td>
</tr>
<tr>
<td>document.hasAttributes()</td>
	<td>文档没有该属性</td>
</tr>
<tr>
<td>document.nextSibling</td>
	<td>文档没有下一节点</td>
</tr>
<tr>
<td>document.nodeName</td>
	<td>这个通常是 #document</td>
</tr>
<tr>
<td>document.nodeType</td>
	<td>这个通常是 9(DOCUMENT_NODE) </td>
</tr>
<tr>
<td>document.nodeValue</td>
	<td>文档没有一个节点值</td>
</tr>
<tr>
<td>document.ownerDocument</td>
	<td>文档没有主文档</td>
</tr>
<tr>
<td>document.ownerElement</td>
	<td>文档没有自己的节点</td>
</tr>
<tr>
<td>document.parentNode</td>
	<td>文档没有父节点</td>
</tr>
<tr>
<td>document.previousSibling</td>
	<td>文档没有兄弟节点</td>
</tr>
<tr>
<td>document.textContent</td>
	<td>文档没有文本节点</td>
</tr>
</tbody></table>			
