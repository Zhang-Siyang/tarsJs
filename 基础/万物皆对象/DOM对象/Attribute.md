<div class="article-intro" id="content">
<h2>HTML DOM 节点</h2>
<p>在 HTML DOM (Document Object Model) 中, 所有的都是  <strong>节点</strong>：
</p>
<ul>
<li>文档是文档节点</li>
<li>所有 HTML 元素是元素节点</li>
	<li>所有 HTML 属性都是属性节点</li>
	<li>插入到 HTML 元素中的文本为文本节点</li>
	<li>注释是注释节点</li>
</ul>
<hr>
<h2>Attr 对象</h2>
<p>在 HTML DOM 中, <strong>Attr 对象</strong> 代表一个 HTML 属性。</p>
<p>HTML属性总是属于HTML元素。</p>

<hr>
<h2>NamedNodeMap 对象</h2>
<p>在 HTML DOM 中, the <strong>NamedNodeMap 对象</strong> 表示一个无顺序的节点列表。</p>
<p>我们可通过节点名称来访问 NamedNodeMap 中的节点。</p>

<hr>
<h2>浏览器支持</h2>
<p>
<p>所有主流浏览器都支持 Attr 对象和 NamedNodeMap 对象。</p>
<hr>
<h2属性和方法< h2="">
<table class="reference">
<tbody><tr>
<th width="30%" align="left">属性 / 方法</th>
<th align="left">描述</th>
</tr>
<tr>
<td><a href="prop-attr-isid.html"><em>attr</em>.isId</a></td>
	<td>如果属性是 ID 类型，则 isId 属性返回 true，否则返回 false。
</td>
</tr>
<tr>
<td><a href="prop-attr-name.html"><em>attr</em>.name</a></td>
	<td>返回属性名称</td>
</tr>
<tr>
<td><a href="prop-attr-value.html"><em>attr</em>.value</a></td>
	<td>设置或者返回属性值</td>
</tr>
<tr>
<td><a href="prop-attr-specified.html"><em>attr</em>.specified</a></td>
	<td>如果属性被指定返回 true
	，否则返回 false
</td>
</tr>
<tr>
<td>&nbsp;</td>
	<td>&nbsp;</td>
</tr>
<tr>
<td><a href="met-namednodemap-getnameditem.html"><em>nodemap</em>.getNamedItem()</a></td>
	<td>从节点列表中返回的指定属性节点。</td>
</tr>
<tr>
<td><a href="met-namednodemap-item.html"><em>nodemap</em>.item()</a></td>
	<td>返回节点列表中处于指定索引号的节点。</td>
</tr>
<tr>
<td><a href="prop-namednodemap-length.html"><em>nodemap</em>.length</a></td>
	<td>返回节点列表的节点数目。</td>
</tr>
<tr>
<td><a href="met-namednodemap-removenameditem.html"><em>nodemap</em>.removeNamedItem()</a></td>
	<td>删除指定属性节点</td>
</tr>
<tr>
<td><a href="met-namednodemap-setnameditem.html"><em>nodemap</em>.setNamedItem()</a></td>
	<td>设置指定属性节点(通过名称)</td>
</tr>
</tbody></table>
<br><hr>
<h2>DOM 4 警告 !!!</h2>
<p>在 W3C DOM 内核中,  Attr (属性) 对象继承节点对象的所有属性和方法 。</p>
<p>在 DOM 4 中, Attr (属性) 对象不再从节点对象中继承。</p>
<p><strong>从长远的代码质量来考虑，在属性对象中你需要避免使用节点对象属性和方法:</strong></p>

<table class="reference">
<tbody><tr>
<th width="30%" align="left">属性 / 方法</th>
<th align="left">避免原因</th>
</tr>
<tr>
<td>
<i>attr</i>.appendChild()</td>
	<td>属性没有子节点</td>
</tr>
<tr>
<td>
<i>attr</i>.attributes</td>
	<td>属性没有属性</td>
</tr>
<tr>
<td>
<i>attr</i>.baseURI</td>
	<td>使用 document.baseURI 替代</td>
</tr>
<tr>
<td>
<i>attr</i>.childNodes</td>
	<td>属性没有子节点</td>
</tr>
<tr>
<td>
<i>attr</i>.cloneNode()</td>
	<td>使用 attr.value 替代</td>
</tr>
<tr>
<td>
<i>attr</i>.firstChild</td>
	<td>属性没有子节点</td>
</tr>
<tr>
<td>
<i>attr</i>.hasAttributes()</td>
	<td>属性没有属性</td>
</tr>
<tr>
<td>
<i>attr</i>.hasChildNodes</td>
	<td>属性没有子节点</td>
</tr>
<tr>
<td>
<i>attr</i>.insertBefore()</td>
	<td>属性没有子节点</td>
</tr>
<tr>
<td>
<i>attr</i>.isEqualNode()</td>
	<td>没有意义</td>
</tr>
<tr>
<td>
<i>attr</i>.isSameNode()</td>
	<td>没有意义</td>
</tr>
<tr>
<td>
<i>attr</i>.isSupported()</td>
	<td>通常为 true</td>
</tr>
<tr>
<td>
<i>attr</i>.lastChild</td>
	<td>属性没有子节点</td>
</tr>
<tr>
<td>
<i>attr</i>.nextSibling</td>
	<td>属性没有兄弟节点</td>
</tr>
<tr>
<td>
<i>attr</i>.nodeName</td>
	<td>使用 <em>attr</em>.name 替代</td>
</tr>
<tr>
<td>
<i>attr</i>.nodeType</td>
	<td>通常为 2 (ATTRIBUTE-NODE) </td>
</tr>
<tr>
<td>
<i>attr</i>.nodeValue</td>
	<td>使用 <em>attr</em>.value 替代</td>
</tr>
<tr>
<td>
<i>attr</i>.normalize()</td>
	<td>属性没有规范</td>
</tr>
<tr>
<td>
<i>attr</i>.ownerDocument</td>
	<td>通常为你的 HTML 文档</td>
</tr>
<tr>
<td>
<i>attr</i>.ownerElement</td>
	<td>你用来访问属性的 HTML 元素</td>
</tr>
<tr>
<td>
<i>attr</i>.parentNode</td>
	<td>你用来访问属性的 HTML 元素</td>
</tr>
<tr>
<td>
<i>attr</i>.previousSibling</td>
	<td>属性没有兄弟节点</td>
</tr>
<tr>
<td>
<i>attr</i>.removeChild</td>
	<td>属性没有子节点 </td>
</tr>
<tr>
<td>
<i>attr</i>.replaceChild</td>
	<td>属性没有子节点</td>
</tr>
<tr>
<td>
<i>attr</i>.textContent</td>
	<td>使用 <i>attr</i>.value 替代</td>
</tr>
</tbody></table>			
