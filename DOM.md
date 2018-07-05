* ![](https://github.com/TUARAN/PIC/blob/master/js/捕获冒泡.png)

* 审查元素和查看网页源码的区别：审查元素实际上看的是渲染过后的Dom,查看网页源代码实际上看到的是未解析的源代码！

* 在Jquery里面，我们可以看到两种写法:$(function(){}) 和$(document).ready(function(){});
这两个方法的效果都是一样的，都是在dom文档树加载完之后执行一个函数（注意，这里面的文档树加载完不代表全部文件加载完）。
而window.onload是在dom文档树加载完和所有文件加载完之后执行一个函数。也就是说$(document).ready要比window.onload先执行。

* ![](https://github.com/TUARAN/PIC/blob/master/js/click与on（click）.png)

* [html全局属性](http://www.runoob.com/tags/ref-standardattributes.html)
