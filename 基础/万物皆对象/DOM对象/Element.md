<div class="article-intro" id="content">
<h2>元素对象</h2>
<p>在 HTML DOM 中, <strong>元素对象</strong>代表着一个 HTML 元素。</p>
<p>元素对象 的 <strong>子节点</strong>可以是, 可以是元素节点，文本节点，注释节点。</p>
<p><strong>NodeList 对象</strong> 代表了节点列表，类似于 HTML元素的子节点集合。</p>
<p>元素可以有属性。属性属于属性节点（查看下一章节）。</p>

<hr>
<h2>浏览器支持</h2>
<p>
<img src="/images/compatible_ie.gif" width="31" height="30" alt="Internet Explorer" title="Internet Explorer"><img src="/images/compatible_firefox.gif" width="31" height="30" alt="Firefox" title="Firefox"><img src="/images/compatible_opera.gif" width="28" height="30" alt="Opera" title="Opera"><img src="/images/compatible_chrome.gif" width="31" height="30" alt="Google Chrome" title="Google Chrome"><img src="/images/compatible_safari.gif" width="28" height="30" alt="Safari" title="Safari"></p>
<p>所有主流浏览器都支持 元素对象 和 NodeList 对象。.</p>

<hr>
<h2>属性和方法</h2>
<p>以上属性和方法可适用于所有 HTML 元素：</p>
<table class="reference">
<tbody><tr>
<th width="35%" align="left">属性 / 方法</th>
    <th align="left">描述</th>
</tr>
<tr>
<td><a href="prop-html-accesskey.html"><i>element</i>.accessKey</a></td>
    <td>设置或返回accesskey一个元素</td>
</tr>

<tr>
    <td><a href="met-element-addeventlistener.html"><i>element</i>.addEventListener()</a></td>
    <td>向指定元素添加事件句柄</td>
</tr>
<tr>
<td><a href="met-node-appendchild.html"><i>element</i>.appendChild()</a></td>
	<td>为元素添加一个新的子元素</td>
</tr>
<tr>
<td><a href="prop-node-attributes.html"><i>element</i>.attributes</a></td>
	<td>返回一个元素的属性数组</td>
</tr>
<tr>
<td><a href="prop-node-childnodes.html"><i>element</i>.childNodes</a></td>
	<td>返回元素的一个子节点的数组</td>
</tr>
<tr>
<td><a href="/jsref/prop-element-children.html"><i>element</i>.children</a></td>
	<td>返回元素的子元素的集合</td>
</tr>
<tr>
<td><a href="prop-element-classList.html"><i>element</i>.classList</a></td>
    <td>返回元素的类名，作为 DOMTokenList 对象。</td>
</tr>
<tr>
<td><a href="prop-html-classname.html"><i>element</i>.className</a></td>
    <td>设置或返回元素的class属性</td>
</tr>
<tr>
<td>
<i>element</i>.clientHeight</td>
    <td>在页面上返回内容的可视高度（不包括边框，边距或滚动条）</td>
</tr>
<tr>
<td>
<i>element</i>.clientWidth</td>
    <td>在页面上返回内容的可视宽度（不包括边框，边距或滚动条）</td>
</tr>
<tr>
<td><a href="met-node-clonenode.html"><i>element</i>.cloneNode()</a></td>
	<td>克隆某个元素</td>
</tr>
<tr>
<td><a href="met-node-comparedocumentposition.html"><i>element</i>.compareDocumentPosition()</a></td>
	<td>比较两个元素的文档位置。</td>
</tr>

<tr>
	<td><a href="prop-html-contenteditable.html"><i>element</i>.contentEditable</a></td>
	<td>设置或返回元素的内容是否可编辑</td>
</tr>
<tr>
<td><a href="prop-html-dir.html"><i>element</i>.dir</a></td>
    <td>设置或返回一个元素中的文本方向</td>
</tr>
<tr>
<td><a href="prop-node-firstchild.html"><i>element</i>.firstChild</a></td>
	<td>返回元素的第一个子节点</td>
</tr>
<tr>
<td><a href="met-html-focus.html"><i>element</i>.focus()</a></td>
	<td>设置文档或元素获取焦点</td>
</tr>
<tr>
<td><a href="met-element-getattribute.html"><i>element</i>.getAttribute()</a></td>
	<td>返回指定元素的属性值</td>
</tr>
<tr>
<td><a href="met-element-getattributenode.html"><i>element</i>.getAttributeNode()</a></td>
	<td>返回指定属性节点</td>
</tr>
<tr>
<td><a href="met-element-getelementsbytagname.html"><i>element</i>.getElementsByTagName()</a></td>
	<td>返回指定标签名的所有子元素集合。</td>
</tr>
<tr>
<td><a href="met-element-getelementsbyclassname.html"><i>element</i>. getElementsByClassName()</a></td>
	<td>返回文档中所有指定类名的元素集合，作为 NodeList 对象。</td>
</tr>
<tr>
<td>
<i>element</i>.getFeature()</td>
	<td>返回指定特征的执行APIs对象。</td>
</tr>
<tr>
<td>
<i>element</i>.getUserData()</td>
	<td>返回一个元素中关联键值的对象。</td>
</tr>
<tr>
<td><a href="met-element-hasattribute.html"><i>element</i>.hasAttribute()</a></td>
	<td>如果元素中存在指定的属性返回 true，否则返回false。</td>
</tr>
<tr>
<td><a href="met-node-hasattributes.html"><i>element</i>.hasAttributes()</a></td>
	<td>如果元素有任何属性返回true，否则返回false。</td>
</tr>
<tr>
<td><a href="met-node-haschildnodes.html"><i>element</i>.hasChildNodes()</a></td>
	<td>返回一个元素是否具有任何子元素</td>
</tr>
<tr>
<td><a href="met-document-hasfocus.html"><i>element</i>.hasFocus()</a></td>
	<td>返回布尔值，检测文档或元素是否获取焦点</td>
</tr>
<tr>
<td><a href="prop-html-id.html"><i>element</i>.id</a></td>
    <td>设置或者返回元素的 id。</td>
</tr>
<tr>
<td><a href="prop-html-innerhtml.html"><i>element</i>.innerHTML</a></td>
    <td>设置或者返回元素的内容。</td>
</tr>
<tr>
<td><a href="met-node-insertbefore.html"><i>element</i>.insertBefore()</a></td>
	<td>现有的子元素之前插入一个新的子元素</td>
</tr>
<tr>
	<td><a href="prop-html-iscontenteditable.html"><i>element</i>.isContentEditable</a></td>
	<td>如果元素内容可编辑返回 true，否则返回false</td>
</tr>

<tr>
<td><a href="met-node-isdefaultnamespace.html"><i>element</i>.isDefaultNamespace()</a></td>
	<td>如果指定了namespaceURI 返回 true，否则返回 false。</td>
</tr>
<tr>
<td><a href="met-node-isequalnode.html"><i>element</i>.isEqualNode()</a></td>
	<td>检查两个元素是否相等</td>
</tr>
<tr>
<td><a href="met-node-issamenode.html"><i>element</i>.isSameNode()</a></td>
	<td>检查两个元素所有有相同节点。</td>
</tr>
<tr>
<td><a href="met-node-issupported.html"><i>element</i>.isSupported()</a></td>
	<td>如果在元素中支持指定特征返回 true。</td>
</tr>
<tr>
<td><a href="prop-html-lang.html"><i>element</i>.lang</a></td>
    <td>设置或者返回一个元素的语言。</td>
</tr>
<tr>
<td><a href="prop-node-lastchild.html"><i>element</i>.lastChild</a></td>
	<td>返回的最后一个子元素</td>
</tr>
<tr>
<td><a href="prop-node-namespaceuri.html"><i>element</i>.namespaceURI</a></td>
	<td>返回命名空间的 URI。</td>
</tr>
<tr>
<td><a href="prop-node-nextsibling.html"><i>element</i>.nextSibling</a></td>
	<td>返回该元素紧跟的一个节点</td>
</tr>
<tr>
</tr><tr>
<td><a href="prop-element-nextelementsibling.html"><i>element</i>.nextElementSibling</a></td>
	<td>返回指定元素之后的下一个兄弟元素（相同节点树层中的下一个元素节点）。</td>
</tr>
<tr>
<td><a href="prop-node-nodename.html"><i>element</i>.nodeName</a></td>
	<td>返回元素的标记名（大写）</td>
</tr>
<tr>
<td><a href="prop-node-nodetype.html"><i>element</i>.nodeType</a></td>
	<td>返回元素的节点类型</td>
</tr>
<tr>
<td><a href="prop-node-nodevalue.html"><i>element</i>.nodeValue</a></td>
	<td>返回元素的节点值</td>
</tr>
<tr>
<td><a href="met-node-normalize.html"><i>element</i>.normalize()</a></td>
	<td>使得此成为一个"normal"的形式，其中只有结构（如元素，注释，处理指令，CDATA节和实体引用）隔开Text节点，即元素（包括属性）下面的所有文本节点，既没有相邻的文本节点也没有空的文本节点</td>
</tr>
<tr>
<td>
<i>element</i>.offsetHeight</td>
    <td>返回，任何一个元素的高度包括边框和填充，但不是边距</td>
</tr>
<tr>
<td>
<i>element</i>.offsetWidth</td>
    <td>返回元素的宽度，包括边框和填充，但不是边距</td>
</tr>
<tr>
<td>
<i>element</i>.offsetLeft</td>
    <td>返回当前元素的相对水平偏移位置的偏移容器</td>
</tr>
<tr>
<td>
<i>element</i>.offsetParent</td>
    <td>返回元素的偏移容器</td>
</tr>
<tr>
<td>
<i>element</i>.offsetTop</td>
    <td>返回当前元素的相对垂直偏移位置的偏移容器</td>
</tr>
<tr>
<td><a href="prop-node-ownerdocument.html"><i>element</i>.ownerDocument</a></td>
	<td>返回元素的根元素（文档对象）</td>
</tr>
<tr>
<td><a href="prop-node-parentnode.html"><i>element</i>.parentNode</a></td>
	<td>返回元素的父节点</td>
</tr>
<tr>
<td><a href="prop-node-previoussibling.html"><i>element</i>.previousSibling</a></td>
	<td>返回某个元素紧接之前元素</td>
</tr>
<tr>
<td><a href="prop-element-previouselementsibling.html"><i>element</i>.previousElementSibling </a></td>
	<td>返回指定元素的前一个兄弟元素（相同节点树层中的前一个元素节点）。</td>
</tr>
<tr>
    <td><a href="met-element-queryselector.html"><i>element</i>.querySelector()</a></td>
    <td>返回匹配指定 CSS 选择器元素的第一个子元素</td>
</tr>
<tr>
    <td>document.querySelectorAll()</td>
    <td>返回匹配指定 CSS 选择器元素的所有子元素节点列表</td>
</tr>
<tr>
<td><a href="met-element-removeattribute.html"><i>element</i>.removeAttribute()</a></td>
	<td>从元素中删除指定的属性</td>
</tr>
<tr>
<td><a href="met-element-removeattributenode.html"><i>element</i>.removeAttributeNode()</a></td>
	<td>删除指定属性节点并返回移除后的节点。</td>
</tr>
<tr>
<td><a href="met-node-removechild.html"><i>element</i>.removeChild()</a></td>
	<td>删除一个子元素</td>
</tr>
<tr>
	<td><a href="met-element-removeeventlistener.html"><i>element</i>.removeEventListener()</a></td>
	<td>移除由 addEventListener() 方法添加的事件句柄</td>
</tr>
<tr>
<td><a href="met-node-replacechild.html"><i>element</i>.replaceChild()</a></td>
	<td>替换一个子元素</td>
</tr>
<tr>
<td>
<i>element</i>.scrollHeight</td>
    <td>返回整个元素的高度（包括带滚动条的隐蔽的地方）</td>
</tr>
<tr>
<td>
<i>element</i>.scrollLeft</td>
    <td>返回当前视图中的实际元素的左边缘和左边缘之间的距离</td>
</tr>
<tr>
<td>
<i>element</i>.scrollTop</td>
    <td>返回当前视图中的实际元素的顶部边缘和顶部边缘之间的距离</td>
</tr>
<tr>
<td>
<i>element</i>.scrollWidth</td>
    <td>返回元素的整个宽度（包括带滚动条的隐蔽的地方）</td>
</tr>
<tr>
<td><a href="met-element-setattribute.html"><i>element</i>.setAttribute()</a></td>
	<td>设置或者改变指定属性并指定值。</td>
</tr>
<tr>
<td><a href="met-element-setattributenode.html"><i>element</i>.setAttributeNode()</a></td>
	<td>设置或者改变指定属性节点。</td>
</tr>
<tr>
<td>
<i>element</i>.setIdAttribute()</td>
	<td></td>
</tr>
<tr>
<td>
<i>element</i>.setIdAttributeNode()</td>
	<td></td>
</tr>
<tr>
<td>
<i>element</i>.setUserData()</td>
	<td>在元素中为指定键值关联对象。</td>
</tr>
<tr>
<td>
<i>element</i>.style</td>
    <td>设置或返回元素的样式属性</td>
</tr>
<tr>
<td><a href="prop-html-tabindex.html"><i>element</i>.tabIndex</a></td>
    <td>设置或返回元素的标签顺序。</td>
</tr>
<tr>
<td><a href="prop-element-tagname.html"><i>element</i>.tagName</a></td>
	<td>作为一个字符串返回某个元素的标记名（大写）</td>
</tr>
<tr>
<td><a href="prop-node-textcontent.html"><i>element</i>.textContent</a></td>
	<td>设置或返回一个节点和它的文本内容</td>
</tr>
<tr>
<td><a href="prop-html-title.html"><i>element</i>.title</a></td>
    <td>设置或返回元素的title属性</td>
</tr>
<tr>
<td>
<i>element</i>.toString()</td>
    <td>一个元素转换成字符串</td>
</tr>

<tr>
<td><a href="met-nodelist-item.html"><em>nodelist</em>.item()</a></td>
	<td>返回某个元素基于文档树的索引</td>
</tr>
<tr>
<td><a href="prop-nodelist-length.html"><em>nodelist</em>.length</a></td>
	<td>返回节点列表的节点数目。</td>
</tr>
</tbody></table>			
			
</div>
