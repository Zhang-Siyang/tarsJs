<div class="article-intro" id="content">
<h2>HTML DOM 事件</h2>
<p>HTML DOM 事件允许Javascript在HTML文档元素中注册不同事件处理程序。</p>
<p>事件通常与函数结合使用，函数不会在事件发生前被执行！
(如用户点击按钮)。</p>
<p><b>提示：</b> 在 W3C 2 级 DOM 事件中规范了事件模型。</p>
<hr>
<h2>HTML DOM 事件</h2>
<p><b>DOM：</b> 指明使用的 DOM 属性级别。</p>

<h2>鼠标事件</h2>

<table class="reference">
<tbody><tr>
<th width="20%" align="left">属性</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">DOM</th>
  </tr>
<tr>
<td><a href="event-onclick.html">onclick</a></td>
	<td>当用户点击某个对象时调用的事件句柄。</td>
    <td>2</td>
  </tr>
<tr>
	<td><a href="event-oncontextmenu.html">oncontextmenu</a></td>
	<td>在用户点击鼠标右键打开上下文菜单时触发</td>
    <td>&nbsp;</td>
  </tr>
<tr>
<td><a href="event-ondblclick.html">ondblclick</a></td>
	<td>当用户双击某个对象时调用的事件句柄。</td>
    <td>2</td>
  </tr>
<tr>
<td><a href="event-onmousedown.html">onmousedown</a></td>
	<td>鼠标按钮被按下。</td>
    <td>2</td>
  </tr>
<tr>
	<td><a href="event-onmouseenter.html">onmouseenter</a></td>
	<td>当鼠标指针移动到元素上时触发。</td>
    <td>2</td>
  </tr>
<tr>
	<td><a href="event-onmouseleave.html">onmouseleave</a></td>
	<td>当鼠标指针移出元素时触发</td>
    <td>2</td>
  </tr>
<tr>
<td><a href="event-onmousemove.html">onmousemove</a></td>
	<td>鼠标被移动。</td>
    <td>2</td>
  </tr>
<tr>
<td><a href="event-onmouseover.html">onmouseover</a></td>
	<td>鼠标移到某元素之上。</td>
    <td>2</td>
  </tr>
<tr>
<td><a href="event-onmouseout.html">onmouseout</a></td>
	<td>鼠标从某元素移开。</td>
    <td>2</td>
  </tr>
<tr>
<td><a href="event-onmouseup.html">onmouseup</a></td>
	<td>鼠标按键被松开。</td>
    <td>2</td>
  </tr>
</tbody></table>
<h2>键盘事件</h2>

<table class="reference notranslate" id="table2">
<tbody><tr>
<th width="20%" align="left">属性</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">DOM</th>
  </tr>
<tr>
<td><a href="event-onkeydown.html">onkeydown</a></td>
	<td>某个键盘按键被按下。</td>
    <td>2</td>
  </tr>
<tr>
<td><a href="event-onkeypress.html">onkeypress</a></td>
	<td>某个键盘按键被按下并松开。</td>
    <td>2</td>
  </tr>
<tr>
<td><a href="event-onkeyup.html">onkeyup</a></td>
	<td>某个键盘按键被松开。</td>
    <td>2</td>
  </tr>
</tbody></table>
<h2>框架/对象（Frame/Object）事件</h2>

<table class="reference notranslate">
<tbody><tr>
<th width="20%" align="left">属性</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">DOM</th>
  </tr>
<tr>
<td><a href="event-onabort.html">onabort</a></td>
	<td>图像的加载被中断。 ( &lt;object&gt;)</td>
    <td>2</td>
  </tr>
<tr>
	<td><a href="event-onbeforeunload.html">onbeforeunload</a></td>
	<td>该事件在即将离开页面（刷新或关闭）时触发</td>
    <td>2</td>
  </tr>
<tr>
<td><a href="event-onerror.html">onerror</a></td>
	<td>在加载文档或图像时发生错误。 ( &lt;object&gt;, 
	&lt;body&gt;和 &lt;frameset&gt;)</td>
    <td>&nbsp;</td>
  </tr>
<tr>
<td><a href="event-onhashchange.html">onhashchange</a></td>
	<td>该事件在当前 URL 的锚部分发生修改时触发。</td>
    <td>&nbsp;</td>
  </tr>
<tr>
<td><a href="event-onload.html">onload</a></td>
	<td>一张页面或一幅图像完成加载。</td>
    <td>2</td>
  </tr>  <tr>
	<td><a href="event-onpageshow.html">onpageshow</a></td>
	<td>该事件在用户访问页面时触发</td>
    <td></td>
  </tr><tr>
	<td><a href="event-onpagehide.html">onpagehide</a></td>
	<td>该事件在用户离开当前网页跳转到另外一个页面时触发</td>
    <td></td>
  </tr>
<tr>
<td><a href="event-onresize.html">onresize</a></td>
	<td>窗口或框架被重新调整大小。</td>
    <td>2</td>
  </tr>
<tr>
<td><a href="event-onscroll.html">onscroll</a></td>
	<td>当文档被滚动时发生的事件。</td>
    <td>2</td>
  </tr>
<tr>
<td><a href="event-onunload.html">onunload</a></td>
	<td>用户退出页面。 ( 
	&lt;body&gt; 和 &lt;frameset&gt;)</td>
    <td>2</td>
  </tr>
</tbody></table>
<h2>表单事件</h2>
<table class="reference notranslate">
  <tbody><tr>
    <th style="width:20%">属性</th>
    <th>描述</th>
    <th style="width:6%">DOM</th>
  </tr>
  <tr>
	<td><a href="event-onblur.html">onblur</a></td>
	<td>元素失去焦点时触发</td>
    <td>2</td>
  </tr>
  <tr>
	<td><a href="event-onchange.html">onchange</a></td>
	<td>该事件在表单元素的内容改变时触发( &lt;input&gt;, &lt;keygen&gt;, &lt;select&gt;, 和 &lt;textarea&gt;)</td>
    <td>2</td>
  </tr>
  <tr>
	<td><a href="event-onfocus.html">onfocus</a></td>
	<td>元素获取焦点时触发</td>
    <td>2</td>
  </tr>
  <tr>
	<td><a href="event-onfocusin.html">onfocusin</a></td>
	<td>元素即将获取焦点时触发</td>
    <td>2</td>
  </tr>
  <tr>
	<td><a href="event-onfocusout.html">onfocusout</a></td>
	<td>元素即将失去焦点时触发</td>
    <td>2</td>
  </tr>
  <tr>
	<td><a href="event-oninput.html">oninput</a></td>
	<td>元素获取用户输入时触发</td>
    <td>3</td>
  </tr>
  <tr>
	<td><a href="event-onreset.html">onreset</a></td>
	<td>表单重置时触发</td>
    <td>2</td>
  </tr>
  <tr>
	<td><a href="event-onsearch.html">onsearch</a></td>
	<td>用户向搜索域输入文本时触发 ( 
	&lt;input="search"&gt;)</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-onselect.html">onselect</a></td>
	<td>用户选取文本时触发 ( &lt;input&gt; 和 &lt;textarea&gt;)</td>
    <td>2</td>
  </tr>
  <tr>
	<td><a href="event-onsubmit.html">onsubmit</a></td>
	<td>表单提交时触发</td>
    <td>2</td>
  </tr>
</tbody></table>
<h2>剪贴板事件</h2>
<table class="reference">
  <tbody><tr>
    <th style="width:20%">属性</th>
    <th>描述</th>
    <th style="width:6%">DOM</th>
  </tr>
  <tr>
	<td><a href="event-oncopy.html">oncopy</a></td>
	<td>该事件在用户拷贝元素内容时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-oncut.html">oncut</a></td>
	<td>该事件在用户剪切元素内容时触发</td>
    <td>&nbsp;</td>
  </tr>
   <tr>
	<td><a href="event-onpaste.html">onpaste</a></td>
	<td>该事件在用户粘贴元素内容时触发</td>
    <td>&nbsp;</td>
  </tr>
</tbody></table>
<h2>打印事件</h2>
<table class="reference">
  <tbody><tr>
    <th style="width:20%">属性</th>
    <th>描述</th>
    <th style="width:6%">DOM</th>
  </tr>
  <tr>
	<td><a href="event-onafterprint.html">onafterprint</a></td>
	<td>该事件在页面已经开始打印，或者打印窗口已经关闭时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-onbeforeprint.html">onbeforeprint</a></td>
	<td>该事件在页面即将开始打印时触发</td>
    <td>&nbsp;</td>
  </tr>
</tbody></table>
<h2>拖动事件</h2>
<table class="reference">
  <tbody><tr>
    <th style="width:20%">事件</th>
    <th>描述</th>
    <th style="width:6%">DOM</th>
  </tr>
  <tr>
	<td><a href="event-ondrag.html">ondrag</a></td>
	<td>该事件在元素正在拖动时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-ondragend.html">ondragend</a></td>
	<td>该事件在用户完成元素的拖动时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-ondragenter.html">ondragenter</a></td>
	<td>该事件在拖动的元素进入放置目标时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-ondragleave.html">ondragleave</a></td>
	<td>该事件在拖动元素离开放置目标时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-ondragover.html">ondragover</a></td>
	<td>该事件在拖动元素在放置目标上时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-ondragstart.html">ondragstart</a></td>
	<td>该事件在用户开始拖动元素时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-ondrop.html">ondrop</a></td>
	<td>该事件在拖动元素放置在目标区域时触发</td>
    <td>&nbsp;</td>
  </tr>
</tbody></table>

<h2>多媒体（Media）事件</h2>
<table class="reference">
  <tbody><tr>
    <th style="width:20%">事件</th>
    <th>描述</th>
    <th style="width:6%">DOM</th>
  </tr>
<tr>
<td><a href="event-onabort-media.html">onabort</a></td>
<td>事件在视频/音频（audio/video）终止加载时触发。</td>
    <td>&nbsp;</td>
</tr>
	<tr>
<td><a href="event-oncanplay.html">oncanplay</a></td>
<td>事件在用户可以开始播放视频/音频（audio/video）时触发。</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-oncanplaythrough.html">oncanplaythrough</a></td>
<td>事件在视频/音频（audio/video）可以正常播放且无需停顿和缓冲时触发。</td>
	    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-ondurationchange.html">ondurationchange</a></td>
<td>事件在视频/音频（audio/video）的时长发生变化时触发。</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td>onemptied</td>
<td>当期播放列表为空时触发</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onended.html">onended</a></td>
<td>事件在视频/音频（audio/video）播放结束时触发。</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onerror-media.html">onerror</a></td>
<td>事件在视频/音频（audio/video）数据加载期间发生错误时触发。</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onloadeddata.html">onloadeddata</a></td>
<td>事件在浏览器加载视频/音频（audio/video）当前帧时触发触发。 </td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onloadedmetadata.html">onloadedmetadata</a></td>
<td>事件在指定视频/音频（audio/video）的元数据加载后触发。</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onloadstart.html">onloadstart</a></td>
<td>事件在浏览器开始寻找指定视频/音频（audio/video）触发。 </td>
	    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onpause.html">onpause</a></td>
<td>事件在视频/音频（audio/video）暂停时触发。</td>
    <td>&nbsp;</td>
	</tr>
<tr>
<td><a href="event-onplay.html">onplay</a></td>
<td>事件在视频/音频（audio/video）开始播放时触发。</td>
    <td>&nbsp;</td>
</tr>
<tr>
<td><a href="event-onplaying.html">onplaying</a></td>
<td> 事件在视频/音频（audio/video）暂停或者在缓冲后准备重新开始播放时触发。

</td>
    <td>&nbsp;</td>
</tr>
	<tr>
<td><a href="event-onprogress.html">onprogress</a></td>
<td>事件在浏览器下载指定的视频/音频（audio/video）时触发。 </td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onratechange.html">onratechange</a></td>
<td>事件在视频/音频（audio/video）的播放速度发送改变时触发。</td>
	    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onseeked.html">onseeked</a></td>
<td>事件在用户重新定位视频/音频（audio/video）的播放位置后触发。</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onseeking.html">onseeking</a></td>
<td> 事件在用户开始重新定位视频/音频（audio/video）时触发。</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onstalled.html">onstalled</a></td>
<td>事件在浏览器获取媒体数据，但媒体数据不可用时触发。</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onsuspend.html">onsuspend</a></td>
<td>事件在浏览器读取媒体数据中止时触发。</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-ontimeupdate.html">ontimeupdate</a></td>
<td>事件在当前的播放位置发送改变时触发。</td>
    <td>&nbsp;</td>
	</tr>
	<tr>
<td><a href="event-onvolumechange.html">onvolumechange</a></td>
<td>事件在音量发生改变时触发。</td>
	    <td>&nbsp;</td>
</tr>
<tr>
<td><a href="event-onwaiting.html">onwaiting</a></td>
<td>事件在视频由于要播放下一帧而需要缓冲时触发。 </td>
    <td>&nbsp;</td>
</tr>
</tbody></table>
<h2>动画事件</h2>
<table class="reference">
  <tbody><tr>
    <th style="width:20%">事件</th>
    <th>描述</th>
    <th style="width:6%">DOM</th>
  </tr>
  <tr>
	<td><a href="event-animationend.html">animationend</a></td>
	<td>该事件在 CSS 动画结束播放时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-animationiteration.html">animationiteration</a></td>
	<td>该事件在 CSS 动画重复播放时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-animationstart.html">animationstart</a></td>
	<td>该事件在 CSS 动画开始播放时触发</td>
    <td>&nbsp;</td>
  </tr>
</tbody></table>
<h2>过渡事件</h2>
<table class="reference">
  <tbody><tr>
    <th style="width:20%">事件</th>
    <th>描述</th>
    <th style="width:6%">DOM</th>
  </tr>
  <tr>
	<td><a href="event-transitionend.html">transitionend</a></td>
	<td>该事件在 CSS 完成过渡后触发。</td>
    <td>&nbsp;</td>
  </tr>
</tbody></table>

<h2>其他事件</h2>
<table class="reference">
  <tbody><tr>
    <th style="width:20%">事件</th>
    <th>描述</th>
    <th style="width:6%">DOM</th>
  </tr>
  <tr>
	<td>onmessage</td>
	<td>该事件通过或者从对象(WebSocket, Web Worker, Event Source 或者子 frame 或父窗口)接收到消息时触发
	</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td>onmousewheel</td>
	<td><span class="deprecated">已废弃。</span> 使用
	<a href="event-onwheel.html">onwheel</a> 事件替代</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-ononline.html">ononline</a></td>
	<td>该事件在浏览器开始在线工作时触发。</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-onoffline.html">onoffline</a></td>
	<td>该事件在浏览器开始离线工作时触发。</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td>onpopstate</td>
	<td>该事件在窗口的浏览历史（history 对象）发生改变时触发。</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-onshow.html">onshow</a></td>
	<td>该事件当 &lt;menu&gt; 元素在上下文菜单显示时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td>onstorage</td>
	<td>该事件在 Web Storage(HTML 5 Web 存储)更新时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-ontoggle.html">ontoggle</a></td>
	<td>该事件在用户打开或关闭 &lt;details&gt; 元素时触发</td>
    <td>&nbsp;</td>
  </tr>
  <tr>
	<td><a href="event-onwheel.html">onwheel</a></td>
	<td>该事件在鼠标滚轮在元素上下滚动时触发</td>
    <td>&nbsp;</td>
  </tr>
</tbody></table>


<h2>事件对象</h2> 

<h3>常量</h3>
<table class="reference notranslate" id="table5">
<tbody><tr>
<th width="20%" align="left">静态变量</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">DOM</th>
  </tr>
<tr>
<td>CAPTURING-PHASE</td>
		<td>当前事件阶段为捕获阶段(1)</td>
		<td>1</td>
  </tr>
<tr>
<td>AT-TARGET</td>
		<td>当前事件是目标阶段,在评估目标事件(1)</td>
		<td>2</td>
  </tr>
<tr>
<td>BUBBLING-PHASE</td>
		<td>当前的事件为冒泡阶段 (3)</td>
		<td>3</td>
  </tr>
</tbody></table>
<h3>属性</h3>
<table class="reference">
<tbody><tr>
<th width="20%" align="left">属性</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">DOM</th>
  </tr>
<tr>
<td><a href="event-bubbles.html">bubbles</a></td>
		<td>返回布尔值，指示事件是否是起泡事件类型。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-cancelable.html">cancelable</a></td>
		<td>返回布尔值，指示事件是否可拥可取消的默认动作。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-currenttarget.html">currentTarget</a></td>
		<td>返回其事件监听器触发该事件的元素。</td>
		<td>2</td>
  </tr>
<tr>
<td>eventPhase</td>
		<td>返回事件传播的当前阶段。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-target.html">target</a></td>
		<td>返回触发此事件的元素（事件的目标节点）。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-timestamp.html">timeStamp</a></td>
		<td>返回事件生成的日期和时间。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-type.html">type</a></td>
		<td>返回当前 Event 对象表示的事件的名称。</td>
		<td>2</td>
  </tr>
</tbody></table>
<h3>方法</h3>
<table class="reference notranslate" id="table3">
<tbody><tr>
<th width="20%" align="left">方法</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">DOM</th>
  </tr>
<tr>
<td>initEvent()</td>
		<td>初始化新创建的 Event 对象的属性。</td>
		<td>2</td>
  </tr>
<tr>
<td>preventDefault()</td>
		<td>通知浏览器不要执行与事件关联的默认动作。</td>
		<td>2</td>
  </tr>
<tr>
<td>stopPropagation()</td>
		<td>不再派发事件。</td>
		<td>2</td>
  </tr>
</tbody></table>
<h2>目标事件对象</h2>
<h3>方法</h3>
<table class="reference notranslate" id="table4">
<tbody><tr>
<th width="20%" align="left">方法</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">DOM</th>
  </tr>
<tr>
<td>addEventListener()</td>
		<td>允许在目标事件中注册监听事件(IE8 
		= attachEvent())</td>
		<td>2</td>
  </tr>
<tr>
<td>dispatchEvent()</td>
		<td>允许发送事件到监听器上 (IE8 = 
		fireEvent())</td>
		<td>2</td>
  </tr>
<tr>
<td>removeEventListener()</td>
		<td>运行一次注册在事件目标上的监听事件(IE8 = 
		detachEvent())</td>
		<td>2</td>
  </tr>
</tbody></table>
<h2>事件监听对象</h2>
<h3>方法</h3>
<table class="reference notranslate" id="table6">
<tbody><tr>
<th width="20%" align="left">方法</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">DOM</th>
  </tr>
<tr>
<td>handleEvent()</td>
		<td>把任意对象注册为事件处理程序</td>
		<td>2</td>
  </tr>
</tbody></table>
<h2>文档事件对象</h2>
<h3>方法</h3><table class="reference notranslate" id="table7">
<tbody><tr>
<th width="20%" align="left">方法</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">DOM</th>
  </tr>
<tr>
<td>createEvent()</td>
		<td>&nbsp;</td>
		<td>2</td>
  </tr>
</tbody></table>
<h2>鼠标/键盘事件对象</h2>
<h3>属性</h3>
<table class="reference notranslate">
<tbody><tr>
<th width="20%" align="left">属性</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">DOM</th>
  </tr>
<tr>
<td><a href="event-altkey.html">altKey</a></td>
		<td>返回当事件被触发时，"ALT" 是否被按下。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-button.html">button</a></td>
		<td>返回当事件被触发时，哪个鼠标按钮被点击。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-clientx.html">clientX</a></td>
		<td>返回当事件被触发时，鼠标指针的水平坐标。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-clienty.html">clientY</a></td>
		<td>返回当事件被触发时，鼠标指针的垂直坐标。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-ctrlkey.html">ctrlKey</a></td>
		<td>返回当事件被触发时，"CTRL" 键是否被按下。</td>
		<td>2</td>
  </tr>

<tr><td><a href="event-key-location.html">Location</a></td>
		<td>返回按键在设备上的位置</td>
		<td>3</td>
  </tr>
<tr><td><a href="event-key-charcode.html">charCode</a></td> <td>返回onkeypress事件触发键值的字母代码。</td> <td>2</td> </tr>
<tr><td><a href="event-key-key.html">key</a></td> <td>在按下按键时返回按键的标识符。</td> <td>3</td> </tr>
<tr><td><a href="event-key-keycode.html">keyCode</a></td> <td>返回onkeypress事件触发的键的值的字符代码，或者 onkeydown 或 onkeyup 事件的键的代码。</td> <td>2</td> </tr>
<tr><td><a href="event-key-which.html">which</a></td> <td>返回onkeypress事件触发的键的值的字符代码，或者 onkeydown 或 onkeyup 事件的键的代码。</td> <td>2</td> </tr>
<tr>
<td><a href="event-metakey.html">metaKey</a></td>
		<td>返回当事件被触发时，"meta" 键是否被按下。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-relatedtarget.html">relatedTarget</a></td>
		<td>返回与事件的目标节点相关的节点。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-screenx.html">screenX</a></td>
		<td>返回当某个事件被触发时，鼠标指针的水平坐标。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-screeny.html">screenY</a></td>
		<td>返回当某个事件被触发时，鼠标指针的垂直坐标。</td>
		<td>2</td>
  </tr>
<tr>
<td><a href="event-shiftkey.html">shiftKey</a></td>
		<td>返回当事件被触发时，"SHIFT" 键是否被按下。</td>
		<td>2</td>
  </tr>
</tbody></table>
<h3>方法</h3>
<table class="reference notranslate" id="table8">
<tbody><tr>
<th width="20%" align="left">方法</th>
    <th width="74%" align="left">描述</th>
    <th width="6%" align="left">W3C</th>
  </tr>
<tr>
<td>initMouseEvent()</td>
		<td>初始化鼠标事件对象的值</td>
		<td>2</td>
  </tr>
<tr>
<td>initKeyboardEvent()</td>
		<td>初始化键盘事件对象的值</td>
		<td>3</td>
  </tr>
</tbody></table>			
