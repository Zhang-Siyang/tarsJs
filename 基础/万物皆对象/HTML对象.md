<h2>Style 对象</h2>
<p>Style 对象表示一个个别的样式声明。</p>

<h3>访问 Style 对象</h3>
<p>Style 对象可以从文档的头部区域访问，或者从指定的 HTML 元素访问。</p>
<p>从文档的头部区域访问 style 对象：</p>
<div class="code notranslate"><div>
var x = document.getElementsByTagName("STYLE");
<a target="_blank" class="playitbtn tryitbtnsyntax" href="/try/try.php?filename=tryjsref_style_get">尝试一下</a>
</div></div>
<p>访问一个指定元素的 style 对象：</p>
<div class="code notranslate"><div>
var x = document.getElementById("myH1").style;
<a target="_blank" class="playitbtn tryitbtnsyntax" href="/try/try.php?filename=tryjsref_style_get_elmnt">尝试一下</a>
</div></div>

<h3>创建 Style 对象</h3>
<p>您可以使用 document.createElement() 方法来创建 &lt;style&gt; 元素：</p>
<div class="code notranslate"><div>
var x = document.createElement("STYLE");
<a target="_blank" class="playitbtn tryitbtnsyntax" href="/try/try.php?filename=tryjsref_style_create">尝试一下</a>
</div></div>
<p>您也可以设置一个已有元素的 style 属性：</p>
<div class="code notranslate"><div>
document.getElementById("myH1").style.color = "red";
<a target="_blank" class="playitbtn tryitbtnsyntax" href="/try/try.php?filename=tryjsref_style_create_elmnt">尝试一下</a>
</div></div>
<h2>Style 对象属性</h2>
  
<p>"CSS" 列表示该属性是在哪一个 CSS 版本中定义的（CSS1、CSS2 或 CSS3）。</p>

<table class="reference notranslate">
  <tbody><tr>
    <th style="width:28%;">属性</th>
    <th style="width:67%;">描述</th>
    <th style="width:5%;">CSS</th>
  </tr>
  <tr>
    <td><a href="prop-style-aligncontent.html">alignContent</a></td>
    <td>设置或返回当灵活容器内的各项没有占用所有可用的空间时各项之间的对齐方式（水平）。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-alignitems.html">alignItems</a></td>
    <td>设置或返回灵活容器内的各项的对齐方式。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-alignself.html">alignSelf</a></td>
    <td>设置或返回灵活容器内被选中项目的对齐方式。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-animation.html">animation</a></td>
    <td>是下面除了 animationPlayState 属性之外的其他属性的速记属性。</td>
    <td>3</td>
  </tr>
    <tr>
    <td><a href="prop-style-animationdelay.html">animationDelay</a></td>
    <td>设置或返回动画何时开始。</td>
    <td>3</td>
    </tr>
    <tr>
    <td><a href="prop-style-animationdirection.html">animationDirection</a></td>
    <td>设置或返回是否循环交替反向播放动画。</td>
    <td>3</td>
    </tr>
	<tr>
    <td><a href="prop-style-animationduration.html">animationDuration</a></td>
    <td>设置或返回动画完成需花费的秒数或毫秒数。</td>
    <td>3</td>
    </tr>
	<tr>
    <td><a href="prop-style-animationfillmode.html">animationFillMode</a></td>
    <td>设置或返回当动画不播放时（当动画完成时，或当动画有一个延迟未开始播放时），要应用到元素的样式。</td>
    <td>3</td>
    </tr>
	<tr>
    <td><a href="prop-style-animationiterationcount.html">animationIterationCount</a></td>
    <td>设置或返回动画的播放次数。</td>
    <td>3</td>
    </tr>
  <tr>
    <td><a href="prop-style-animationname.html">animationName</a></td>
    <td>设置或返回关键帧 @keyframes 动画的名称。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-animationtimingfunction.html">animationTimingFunction</a></td>
    <td>设置或返回动画的速度曲线。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-animationplaystate.html">animationPlayState</a></td>
    <td>设置或返回动画是运行的还是暂停的。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-background.html">background</a></td>
    <td>设置或返回在一个声明中的所有背景属性。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-backgroundattachment.html">backgroundAttachment</a></td>
    <td>设置或返回背景图像是否固定或随页面滚动。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-backgroundcolor.html">backgroundColor</a></td>
    <td>设置或返回元素的背景色。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-backgroundimage.html">backgroundImage</a></td>
    <td>设置或返回元素的背景图像。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-backgroundposition.html">backgroundPosition</a></td>
    <td>设置或返回的背景图像的起始位置。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-backgroundrepeat.html">backgroundRepeat</a></td>
    <td>设置或返回如何重复背景图像。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-backgroundclip.html">backgroundClip</a></td>
    <td>设置或返回背景的绘制区域。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-backgroundorigin.html">backgroundOrigin</a></td>
    <td>设置或返回背景图像的定位区域。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-backgroundsize.html">backgroundSize</a></td>
    <td>设置或返回背景图像的大小。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-backfacevisibility.html">backfaceVisibility</a></td>
    <td>设置或返回当一个元素背对屏幕时是否可见。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-border.html">border</a></td>
    <td>设置或返回在一个声明中的 borderWidth、borderStyle 和 borderColor。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderbottom.html">borderBottom</a></td>
    <td>设置或返回在一个声明中的所有 borderBottom* 属性。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderbottomcolor.html">borderBottomColor</a></td>
    <td>设置或返回下边框的颜色。</td>
    <td>1&nbsp;</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderbottomleftradius.html">borderBottomLeftRadius</a></td>
    <td>设置或返回左下角边框的形状。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderbottomrightradius.html">borderBottomRightRadius</a></td>
    <td>设置或返回右下角边框的形状。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderbottomstyle.html">borderBottomStyle</a></td>
    <td>设置或返回下边框的样式。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderbottomwidth.html">borderBottomWidth</a></td>
    <td>设置或返回下边框的宽度。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-bordercollapse.html">borderCollapse</a></td>
    <td>设置或返回表格的边框是否被折叠为一个单一的边框。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-bordercolor.html">borderColor</a></td>
    <td>设置或返回元素边框的颜色（最多可以有四个值）。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderimage.html">borderImage</a></td>
    <td>一个用于设置或返回所有的 borderImage* 属性的速记属性。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderimageoutset.html">borderImageOutset</a></td>
    <td>设置或返回边框图像区域超出边界框的量。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderimagerepeat.html">borderImageRepeat</a></td>
    <td>设置或返回图像边框是重复拼接图块还是延伸图块。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderimageslice.html">borderImageSlice</a></td>
    <td>设置或返回图像边框的向内偏移。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderimagesource.html">borderImageSource</a></td>
    <td>设置或返回要作为边框使用的图像。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderimagewidth.html">borderImageWidth</a></td>
    <td>设置或返回图像边框的宽度。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderleft.html">borderLeft</a></td>
    <td>设置或返回在一个声明中的所有 borderLeft* 属性。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderleftcolor.html">borderLeftColor</a></td>
    <td>设置或返回左边框的颜色。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderleftstyle.html">borderLeftStyle</a></td>
    <td>设置或返回左边框的样式。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderleftwidth.html">borderLeftWidth</a></td>
    <td>设置或返回左边框的宽度。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderradius.html">borderRadius</a></td>
    <td>一个用于设置或返回四个 border*Radius 属性的速记属性。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderright.html">borderRight</a></td>
    <td>设置或返回在一个声明中的所有 borderRight* 属性。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderrightcolor.html">borderRightColor</a></td>
    <td>设置或返回右边框的颜色。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderrightstyle.html">borderRightStyle</a></td>
    <td>设置或返回右边框的样式。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderrightwidth.html">borderRightWidth</a></td>
    <td>设置或返回右边框的宽度。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderspacing.html">borderSpacing</a></td>
    <td>设置或返回表格中单元格之间的距离。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderstyle.html">borderStyle</a></td>
    <td>设置或返回元素边框的样式（最多可以有四个值）。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-bordertop.html">borderTop</a></td>
    <td>设置或返回在一个声明中的所有 borderTop* 属性。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-bordertopcolor.html">borderTopColor</a></td>
    <td>设置或返回上边框的颜色。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-bordertopleftradius.html">borderTopLeftRadius</a></td>
    <td>设置或返回左上角边框的形状。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-bordertoprightradius.html">borderTopRightRadius</a></td>
    <td>设置或返回右上角边框的形状。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-bordertopstyle.html">borderTopStyle</a></td>
    <td>设置或返回上边框的样式。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-bordertopwidth.html">borderTopWidth</a></td>
    <td>设置或返回上边框的宽度。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-borderwidth.html">borderWidth</a></td>
    <td>设置或返回元素边框的宽度（最多可以有四个值）。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-bottom.html">bottom</a></td>
    <td>设置或返回定位元素的底部位置。</td>
    <td>2</td>
  </tr>
  <tr>
    <td>boxDecorationBreak</td>
    <td>设置或返回分页处元素的背景和边框行为，或者换行处内联元素的背景和边框行为。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-boxshadow.html">boxShadow</a></td>
    <td>设置或返回元素的下拉阴影。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-boxsizing.html">boxSizing</a></td>
    <td>允许您以特定的方式定义匹配某个区域的特定元素。</td>
    <td>3</td>
  </tr>
<!--
  <tr>
    <td>breakAfter</td>
    <td></td>
    <td>3</td>
  </tr>
  <tr>
    <td>breakBefore</td>
    <td></td>
    <td>3</td>
  </tr>
  <tr>
    <td>breakInside</td>
    <td></td>
    <td>3</td>
  </tr>
-->
  <tr>
    <td><a href="prop-style-captionside.html">captionSide</a></td>
    <td>设置或返回表格标题的位置。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-clear.html">clear</a></td>
    <td>设置或返回元素相对浮动对象的位置。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-clip.html">clip</a></td>
    <td>设置或返回定位元素的可见部分。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-color.html">color</a></td>
    <td>设置或返回文本的颜色。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-columncount.html">columnCount</a></td>
    <td>设置或返回元素应该被划分的列数。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-columnfill.html">columnFill</a></td>
    <td>设置或返回如何填充列。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-columngap.html">columnGap</a></td>
    <td>设置或返回列之间的间隔。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-columnrule.html">columnRule</a></td>
    <td>一个用于设置或返回所有的 columnRule* 属性的速记属性。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-columnrulecolor.html">columnRuleColor</a></td>
    <td>设置或返回列之间的颜色规则。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-columnrulestyle.html">columnRuleStyle</a></td>
    <td>设置或返回列之间的样式规则。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-columnrulewidth.html">columnRuleWidth</a></td>
    <td>设置或返回列之间的宽度规则。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-columns.html">columns</a></td>
    <td>一个用于设置或返回 columnWidth 和 columnCount 的速记属性。</td>
    <td>3</td>
  </tr>  
  <tr>
    <td><a href="prop-style-columnspan.html">columnSpan</a></td>
    <td>设置或返回一个元素应横跨多少列。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-columnwidth.html">columnWidth</a></td>
    <td>设置或返回列的宽度。</td>
    <td>3</td>
  </tr>
  <tr>
    <td>content</td>
    <td>与 :before 和 :after 伪元素一起使用，来插入生成的内容。</td>
    <td>2</td>
  </tr>  
  <tr>
    <td><a href="prop-style-counterincrement.html">counterIncrement</a></td>
    <td>增加一个或多个计数器。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-counterreset.html">counterReset</a></td>
    <td>创建或重置一个或多个计数器。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-cursor.html">cursor</a></td>
    <td>设置或返回鼠标指针显示的光标类型。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-direction.html">direction</a></td>
    <td>设置或返回文本的方向。</td>
    <td>2</td>
  </tr>
	<tr>
    <td><a href="prop-style-display.html">display</a></td>
    <td>设置或返回元素的显示类型。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-emptycells.html">emptyCells</a></td>
    <td>设置或返回是否显示表格中的空单元格的边框和背景。</td>
    <td>2</td>
  </tr>
<tr>
    <td><a href="prop-style-filter.html">filter</a></td>
    <td>设置或返回图片滤镜(可视效果，如：高斯模糊与饱和度)</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-flex.html">flex</a></td>
    <td>相对于同一容器其他灵活的项目，设置或返回项目的长度。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-flexbasis.html">flexBasis</a></td>
    <td>设置或灵活项目的初始长度。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-flexdirection.html">flexDirection</a></td>
    <td>设置或返回灵活项目的方向。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-flexflow.html">flexFlow</a></td>
    <td>是 flexDirection 和 flexWrap 属性的速记属性。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-flexgrow.html">flexGrow</a></td>
    <td>设置或返回项目将相对于同一容器内其他灵活的项目进行扩展的量。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-flexshrink.html">flexShrink</a></td>
    <td>设置或返回项目将相对于同一容器内其他灵活的项目进行收缩的量。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-flexwrap.html">flexWrap</a></td>
    <td>设置或返回灵活项目是否拆行或拆列。</td>
    <td>3</td>
  </tr>
	<tr>
    <td><a href="prop-style-cssfloat.html">cssFloat</a></td>
    <td>设置或返回元素的水平对齐方式。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-font.html">font</a></td>
    <td>设置或返回一个声明中的 fontStyle、fontVariant、fontWeight、fontSize、lineHeight 和 fontFamily。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-fontfamily.html">fontFamily</a></td>
    <td>设置或返回文本的字体。</td>
    <td>1</td>
  </tr>
<!--
  <tr>
    <td>fontFeatureSetting</td>
    <td></td>
    <td>3</td>
  </tr>
  <tr>
    <td>fontKerning</td>
    <td></td>
    <td>3</td>
  </tr> 
  <tr>
    <td>fontLanguageOverride</td>
    <td></td>
    <td>3</td>
  </tr> 
  <tr>
    <td>fontSynthesis</td>
    <td></td>
    <td>3</td>
  </tr> 
  <tr>
    <td>fontVariantAlternates</td>
    <td></td>
    <td>3</td>
  </tr> 
  <tr>
    <td>fontVariantCaps</td>
    <td></td>
    <td>3</td>
  </tr> 
  <tr>
    <td>fontVariantEastAsian</td>
    <td></td>
    <td>3</td>
  </tr> 
  <tr>
    <td>fontVariantLigatures</td>
    <td></td>
    <td>3</td>
  </tr> 
  <tr>
    <td>fontVariantNumeric</td>
    <td></td>
    <td>3</td>
  </tr> 
  <tr>
    <td>fontVariantPosition</td>
    <td></td>
    <td>3</td>
  </tr> 
-->
  <tr>
    <td><a href="prop-style-fontsize.html">fontSize</a></td>
    <td>设置或返回文本的字体尺寸。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-fontstyle.html">fontStyle</a></td>
    <td>设置或返回字体样式是否是 normal（正常的）、italic（斜体）或 oblique（倾斜的）。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-fontvariant.html">fontVariant</a></td>
    <td>设置或返回是否以小型大写字母显示字体。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-fontweight.html">fontWeight</a></td>
    <td>设置或返回字体的粗细。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-fontsizeadjust.html">fontSizeAdjust</a></td>
    <td>当使用备用字体时，确保文本的可读性。</td>
    <td>3</td>
  </tr>
  <tr>
    <td>fontStretch</td>
    <td>从字体库中选择一种正常的、浓缩的或扩大的字体。</td>
    <td>3</td>
  </tr>
  <tr>
    <td>hangingPunctuation</td>
    <td>规定一个标点符号是否可以放置在线框外。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-height.html">height</a></td>
    <td>设置或返回元素的高度。</td>
    <td>1</td>
  </tr>
  <tr>
    <td>hyphens</td>
    <td>设置如何拆分单词来提高段落布局。</td>
    <td>3</td>
  </tr>  
	<tr>
    <td>icon</td>
    <td>向作者提供为一个带有等价于图标的元素定义样式的功能。</td>
    <td>3</td>
  </tr>  
  <tr>
    <td>imageOrientation</td>
    <td>规定一个用户代理应用到图像上的顺时针方向的旋转。</td>
    <td>3</td>
  </tr>
<!--
  <tr>
    <td>imageRendering</td>
    <td></td>
    <td>3</td>
  </tr>
  <tr>
    <td>imageResolution</td>
    <td></td>
    <td>3</td>
  </tr>
	<tr>
    <td>imeMode</td>
    <td></td>
    <td>3</td>
  </tr>  
-->
  <tr>
    <td><a href="prop-style-justifycontent.html">justifyContent</a></td>
    <td>设置或返回当灵活容器内的各项没有占用所有可用的空间时各项之间的对齐方式（垂直）。</td>
    <td>3</td>
  </tr>  
  <tr>
    <td><a href="prop-style-left.html">left</a></td>
    <td>设置或返回定位元素的左部位置。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-letterspacing.html">letterSpacing</a></td>
    <td>设置或返回文本中字符之间的空间。</td>
    <td>1</td>
  </tr>
<!--
  <tr>
    <td>lineBreak</td>
    <td></td>
    <td>3</td>
  </tr>
-->
  <tr>
    <td><a href="prop-style-lineheight.html">lineHeight</a></td>
    <td>设置或返回在文本中行之间的距离。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-liststyle.html">listStyle</a></td>
    <td>设置或返回一个声明中的 listStyleImage、listStylePosition 和 listStyleType。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-liststyleimage.html">listStyleImage</a></td>
    <td>设置或返回作为列表项标记的图像。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-liststyleposition.html">listStylePosition</a></td>
    <td>设置或返回列表项标记的位置。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-liststyletype.html">listStyleType</a></td>
    <td>设置或返回列表项标记的类型。</td>
    <td>1</td>
  </tr>  
  <tr>
    <td><a href="prop-style-margin.html">margin</a></td>
    <td>设置或返回元素的外边距（最多可以有四个值）。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-marginbottom.html">marginBottom</a></td>
    <td>设置或返回元素的的下外边距。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-marginleft.html">marginLeft</a></td>
    <td>设置或返回元素的左外边距。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-marginright.html">marginRight</a></td>
    <td>设置或返回元素的右外边距。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-margintop.html">marginTop</a></td>
    <td>设置或返回元素的上外边距。</td>
    <td>1</td>
  </tr>
<!--
  <tr>
    <td>mark</td>
    <td>A shorthand property for setting the mark-before and mark-after properties</td>
    <td>3</td>
  </tr>
	<tr>
    <td>markAfter</td>
    <td>Allows named markers to be attached to the audio stream</td>
    <td>3</td>
  </tr>
	<tr>
    <td>markBefore</td>
    <td>Allows named markers to be attached to the audio stream</td>
    <td>3</td>
  </tr>
  <tr>
    <td>marks</td>
    <td>Adds crop and/or cross marks to the document</td>
    <td>3</td>
  </tr>
  <tr>
    <td>marqueeDirection</td>
    <td>Sets the direction of the moving content</td>
    <td>3</td>
  </tr>
  <tr>
    <td>marqueePlayCount</td>
    <td>Sets how many times the content move</td>
    <td>3</td>
  </tr>
  <tr>
    <td>marqueeSpeed</td>
    <td>Sets how fast the content scrolls</td>
    <td>3</td>
  </tr>
  <tr>
    <td>marqueeStyle</td>
    <td>Sets the style of the moving content</td>
    <td>3</td>
  </tr>
  <tr>
    <td>mask</td>
    <td></td>
    <td>3</td>
  </tr>
  <tr>
    <td>maskType</td>
    <td></td>
    <td>3</td>
  </tr>  
-->
  <tr>
    <td><a href="prop-style-maxheight.html">maxHeight</a></td>
    <td>设置或返回元素的最大高度。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-maxwidth.html">maxWidth</a></td>
    <td>设置或返回元素的最大宽度。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-minheight.html">minHeight</a></td>
    <td>设置或返回元素的最小高度。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-minwidth.html">minWidth</a></td>
    <td>设置或返回元素的最小宽度。</td>
    <td>2</td>
  </tr>
	<tr>
    <td>navDown</td>
    <td>设置或返回当使用向下箭头导航键时要导航到哪里。</td>
    <td>3</td>
  </tr>
	<tr>
    <td>navIndex</td>
    <td>设置或返回元素的显示顺序。</td>
    <td>3</td>
  </tr>
	<tr>
    <td>navLeft</td>
    <td>设置或返回当使用向左箭头导航键时要导航到哪里。</td>
    <td>3</td>
  </tr>
	<tr>
    <td>navRight</td>
    <td>设置或返回当使用向右箭头导航键时要导航到哪里。</td>
    <td>3</td>
  </tr>
  <tr>
    <td>navUp</td>
    <td>设置或返回当使用向上箭头导航键时要导航到哪里。</td>
    <td>3</td>
  </tr>
<!--
  <tr>
    <td>objectFit</td>
    <td></td>
    <td>3</td>
  </tr>
  <tr>
    <td>objectPosition</td>
    <td></td>
    <td>3</td>
  </tr>
-->
  <tr>
    <td><a href="prop-style-opacity.html">opacity</a></td>
    <td>设置或返回元素的不透明度。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-order.html">order</a></td>
    <td>设置或返回一个灵活的项目相对于同一容器内其他灵活项目的顺序。</td>
    <td>3</td>
  </tr>    
  <tr>
    <td><a href="prop-style-orphans.html">orphans</a></td>
    <td>设置或返回当元素内有分页时，必须在页面底部预留的最小行数。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-outline.html">outline</a></td>
    <td>设置或返回在一个声明中的所有 outline 属性。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-outlinecolor.html">outlineColor</a></td>
    <td>设置或返回一个元素周围的轮廓颜色。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-outlineoffset.html">outlineOffset</a></td>
    <td>对轮廓进行偏移，并在边框边缘进行绘制。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-outlinestyle.html">outlineStyle</a></td>
    <td>设置或返回一个元素周围的轮廓样式。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-outlinewidth.html">outlineWidth</a></td>
    <td>设置或返回一个元素周围的轮廓宽度。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-overflow.html">overflow</a></td>
    <td>设置或返回如何处理呈现在元素框外面的内容。</td>
    <td>2</td>
  </tr>
<!--
  <tr>
    <td>overflowWrap</td>
    <td></td>
    <td>3</td>
  </tr>  
-->
  <tr>
    <td><a href="prop-style-overflowx.html">overflowX</a></td>
    <td>规定如果内容溢出元素的内容区域，是否对内容的左/右边缘进行裁剪。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-overflowy.html">overflowY</a></td>
    <td>规定如果内容溢出元素的内容区域，是否对内容的上/下边缘进行裁剪。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-padding.html">padding</a></td>
    <td>设置或返回元素的内边距（最多可以有四个值）。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-paddingbottom.html">paddingBottom</a></td>
    <td>设置或返回元素的下内边距。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-paddingleft.html">paddingLeft</a></td>
    <td>设置或返回元素的左内边距。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-paddingright.html">paddingRight</a></td>
    <td>设置或返回元素的右内边距。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-paddingtop.html">paddingTop</a></td>
    <td>设置或返回元素的上内边距。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-pagebreakafter.html">pageBreakAfter</a></td>
    <td>设置或返回元素后的分页行为。</td>
    <td>2</td>
  </tr>
	<tr>
    <td><a href="prop-style-pagebreakbefore.html">pageBreakBefore</a></td>
    <td>设置或返回元素前的分页行为。</td>
    <td>2</td>
  </tr>
	<tr>
    <td><a href="prop-style-pagebreakinside.html">pageBreakInside</a></td>
    <td>设置或返回元素内的分页行为。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-perspective.html">perspective</a></td>
    <td>设置或返回 3D 元素被查看的视角。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-perspectiveorigin.html">perspectiveOrigin</a></td>
    <td>设置或返回 3D 元素的底部位置。</td>
    <td>3</td>
  </tr>
<!--
	<tr>
    <td>phonemes</td>
    <td>Specifies a phonetic pronunciation for the text contained by the corresponding element</td>
    <td>3</td>
  </tr>
-->
  <tr>
    <td><a href="prop-style-position.html">position</a></td>
    <td>设置或返回用于元素定位方法的类型（static、relative、absolute 或 fixed）。</td>
    <td>2</td>
  </tr>  
  <tr>
    <td><a href="prop-style-quotes.html">quotes</a></td>
    <td>设置或返回嵌入引用的引号类型。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-resize.html">resize</a></td>
    <td>设置或返回是否可由用户调整元素的尺寸大小。</td>
    <td>3</td>
  </tr>
<!--
	<tr>
    <td>rest</td>
    <td>A shorthand property for setting the rest-before and rest-after properties </td>
    <td>3</td>
  </tr>
	<tr>
    <td>restAfter</td>
    <td>Specifies a rest or prosodic boundary to be observed after speaking an element's content</td>
    <td>3</td>
  </tr>
  <tr>
    <td>restBefore</td>
    <td>Specifies a rest or prosodic boundary to be observed before speaking an element's content</td>
    <td>3</td>
  </tr>
-->
  <tr>
    <td><a href="prop-style-right.html">right</a></td>
    <td>设置或返回定位元素的右部位置。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-tablelayout.html">tableLayout</a></td>
    <td>设置或返回表格单元格、行、列的布局方式。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-tabsize.html">tabSize</a></td>
    <td>设置或返回制表符（tab）字符的长度。</td>
    <td>3</td>
  </tr>  
  <tr>
    <td><a href="prop-style-textalign.html">textAlign</a></td>
    <td>设置或返回文本的水平对齐方式。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-textalignlast.html">textAlignLast</a></td>
    <td>设置或返回当 text-align 属性设置为 "justify" 时，如何对齐一个强制换行符前的最后一行。</td>
    <td>3</td>
  </tr> 
<!--
  <tr>
    <td>textCombineHorizontal</td>
    <td></td>
    <td>3</td>
  </tr>     
-->
  <tr>
    <td><a href="prop-style-textdecoration.html">textDecoration</a></td>
    <td>设置或返回文本的修饰。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-textdecorationcolor.html">textDecorationColor</a></td>
    <td>设置或返回文本修饰的颜色。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-textdecorationline.html">textDecorationLine</a></td>
    <td>设置或返回文本修饰要使用的线条类型。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-textdecorationstyle.html">textDecorationStyle</a></td>
    <td>设置或返回文本修饰中的线条样式。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-textindent.html">textIndent</a></td>
    <td>设置或返回文本第一行的缩进。</td>
    <td>1</td>
  </tr>
  <tr>
    <td>textJustify</td>
    <td>设置或返回当 text-align 属性设置为 "justify" 时，要使用的对齐方法。</td>
    <td>3</td>
  </tr>
<!--
  <tr>
    <td>textOrientation</td>
    <td></td>
    <td>3</td>
  </tr>     
-->
  <tr>
    <td><a href="prop-style-textoverflow.html">textOverflow</a></td>
    <td>设置或返回当文本溢出包含它的元素，应该发生什么。</td>
    <td>3</td>
  </tr> 
  <tr>
    <td><a href="prop-style-textshadow.html">textShadow</a></td>
    <td>设置或返回文本的阴影效果。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-texttransform.html">textTransform</a></td>
    <td>设置或返回文本的大小写。</td>
    <td>1</td>
  </tr>
<!--
  <tr>
    <td>textUnderlinePosition</td>
    <td></td>
    <td>3</td>
  </tr>
-->
  <tr>
    <td><a href="prop-style-top.html">top</a></td>
    <td>设置或返回定位元素的顶部位置。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-transform.html">transform</a></td>
    <td>向元素应用 2D 或 3D 转换。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-transformorigin.html">transformOrigin</a></td>
    <td>设置或返回被转换元素的位置。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-transformstyle.html">transformStyle</a></td>
    <td>设置或返回被嵌套的元素如何呈现在 3D 空间中。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-transition.html">transition</a></td>
    <td>一个用于设置或返回四个过渡属性的速记属性。</td>
    <td>3</td>
  </tr>
	<tr>
    <td><a href="prop-style-transitionproperty.html">transitionProperty</a></td>
    <td>应用过渡效果的 CSS 属性的名称。</td>
    <td>3</td>
  </tr>
	<tr>
    <td><a href="prop-style-transitionduration.html">transitionDuration</a></td>
    <td>设置或返回完成过渡效果需要花费的时间（以秒或毫秒计）。</td>
    <td>3</td>
  </tr>
	<tr>
    <td><a href="prop-style-transitiontimingfunction.html">transitionTimingFunction</a></td>
    <td>设置或返回过渡效果的速度曲线。</td>
    <td>3</td>
  </tr>
	<tr>
    <td><a href="prop-style-transitiondelay.html">transitionDelay</a></td>
    <td>设置或返回过渡效果何时开始。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-unicodebidi.html">unicodeBidi</a></td>
    <td>设置或返回文本是否被重写，以便在同一文档中支持多种语言。</td>
    <td>2</td>
  </tr>
  <tr>
    <td><a href="prop-style-verticalalign.html">verticalAlign</a></td>
    <td>设置或返回元素中内容的垂直对齐方式。</td>
    <td>1</td>
  </tr>    
  <tr>
    <td><a href="prop-style-visibility.html">visibility</a></td>
    <td>设置或返回元素是否应该是可见的。</td>
    <td>2</td>
  </tr>
<!--
  <tr>
    <td>voiceBalance</td>
    <td>Specifies the balance between left and right channels</td>
    <td>3</td>
  </tr>
  <tr>
    <td>voiceDuration</td>
    <td>Specifies how long it should take to render the selected element's content</td>
    <td>3</td>
  </tr>
  <tr>
    <td>voicePitch</td>
    <td>Specifies the average pitch (a frequency) of the speaking voice</td>
    <td>3</td>
  </tr>
  <tr>
    <td>voicePitchRange</td>
    <td>Specifies variation in average pitch</td>
    <td>3</td>
  </tr>
  <tr>
    <td>voiceRate</td>
    <td>Controls the speaking rate</td>
    <td>3</td>
  </tr>
  <tr>
    <td>voiceStress</td>
    <td>Indicates the strength of emphasis to be applied</td>
    <td>3</td>
  </tr>
  <tr>
    <td>voiceVolume</td>
    <td>Refers to the amplitude of the waveform output by the speech synthesises</td>
    <td>3</td>
  </tr>
-->
  <tr>
    <td><a href="prop-style-whitespace.html">whiteSpace</a></td>
    <td>设置或返回如何处理文本中的制表符、换行符和空格符。</td>
    <td>1</td>
  </tr>  
  <tr>
    <td><a href="prop-style-width.html">width</a></td>
    <td>设置或返回元素的宽度。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-wordbreak.html">wordBreak</a></td>
    <td>设置或返回非 CJK 语言的换行规则。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-wordspacing.html">wordSpacing</a></td>
    <td>设置或返回文本中单词之间的空间。</td>
    <td>1</td>
  </tr>
  <tr>
    <td><a href="prop-style-wordwrap.html">wordWrap</a></td>
    <td>允许长单词或 URL 地址换行到下一行。</td>
    <td>3</td>
  </tr>
  <tr>
    <td><a href="prop-style-widows.html">widows</a></td>
    <td>设置或返回一个元素必须在页面顶部的可见行的最小数量。</td>
    <td>2</td>
  </tr>
<!--
  <tr>
    <td>writingMode</td>
    <td></td>
    <td>3</td>
  </tr>     
-->
  <tr>
    <td><a href="prop-style-zindex.html">zIndex</a></td>
    <td>设置或返回定位元素的堆叠顺序。</td>
    <td>2</td>
  </tr>
</tbody></table>		
