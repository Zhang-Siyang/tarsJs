# 1
>快速获取文档元素

>提供漂亮的页面动态效果

>创建AJAX无刷新网页

>提供对JavaScript语言的增强

>增强的事件处理

>更改网页内容
# 2
```
定义和用法
delegate() 方法为指定的元素（属于被选元素的子元素）添加一个或多个事件处理程序，并规定当这些事件发生时运行的函数。

使用 delegate() 方法的事件处理程序适用于当前或未来的元素（比如由脚本创建的新元素）。

语法
$(selector).delegate(childSelector,event,data,function)
```

# 3
```
通过 closest() 完成事件委托。当被最接近的列表元素或其子后代元素被点击时，会切换黄色背景：

$( document ).bind("click", function( e ) {
    $( e.target ).closest("li").toggleClass("hilight");
  });

定义和用法
closest() 方法获得匹配选择器的第一个祖先元素，从当前元素开始沿 DOM 树向上。

语法
.closest(selector)
```

# 4

名称|用法
-|-
append|A.append(B)，把B加入A的内部的后面。如果B在页面上存在，则删除原来位置的B
appendTo|	B.appendTo(A),同append，只是书写顺序不一样
prepend	|A.prepend(B),把B加入A的内部的前面。如果B在页面上存在，则删除原来位置的B
prependTo	|B.prependTo(A),同prepend

append() - 在被选元素的结尾插入内容

prepend() - 在被选元素的开头插入内容

after() - 在被选元素之后插入内容

before() - 在被选元素之前插入内容
# 5
[jQuery里面的普通绑定事件和on委托事件](https://www.cnblogs.com/wufangfang/p/5333007.html)
```
//hover事件的事件委托：

$('ul').on('mouseenter', 'li', function() {//绑定鼠标进入事件
    $(this).addClass('hover');
});
$('ul').on('mouseleave', 'li', function() {//绑定鼠标划出事件
    $(this).removeClass('hover');
});

```

