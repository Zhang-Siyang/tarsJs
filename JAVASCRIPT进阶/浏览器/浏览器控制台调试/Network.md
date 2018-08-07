
# 概述：性能

[Chrome 开发者工具中文文档](http://www.css88.com/doc/chrome-devtools/network-performance/resource-loading/)

问题：

1.通过浏览器输入网址的行为，统一为“GET”方法；

2.GET提交的数据会在地址栏中显示出来，而POST提交，地址栏不会改变；

3.get是把参数数据队列加到提交表单的ACTION属性所指的URL中，值和表单内各个字段一一对应，在URL中可以看到。
post是通过HTTPpost机制，将表单内各个字段与其内容放置在HTML HEADER内一起传送到ACTION属性所指的URL地址。
用户看不到这个过程。

4.get传送的数据量较小，不能大于2KB。post传送的数据量较大，一般被默认为不受限制

[HTTP Request Header 请求头](https://blog.csdn.net/lipeigang1109/article/details/59057525)

[postman 使用post方式提交参数值](https://www.cnblogs.com/haoxuanchen2014/p/7771459.html  )

5. ### [Cookie](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Cookies)


