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
