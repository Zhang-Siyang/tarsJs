# 1

> Elments面板是所有浏览器调试台的处在第一位置的面板:</br>
opera54.0/chrome67.0/360-10.0(极速) 称之为："Elments"；</br>
firefox61.0 称之为：“查看器”；</br>
IE11 称之为：“DOM资源管理器”；//日期：2018.7.20

[网上说](https://www.cnblogs.com/LibraThinker/p/5948448.html)，它的功能是：“查找网页源代码HTML中的任一元素,手动修改任一元素的属性和样式且能实时在浏览器里面得到反馈。”

# 2

1.“查找网页源代码...”,这样的描述————不够准确，“源代码”是 **服务器端发送到浏览器端的代码（源代码未解析、DOM未渲染）**；而打开控制台的“审查元素”操作看到的代码是 **浏览器执行js动态生成的代码（源码已解析、DOM已渲染）**。 这是关键且明显的差别。可取之处，“查找”二字点明的妥当。

e.g.
![](https://github.com/TUARAN/pic/blob/master/js/elments查.png)


2.“手动修改任一元素的属性和样式且能实时在浏览器里面得到反馈”,这样的描述————还行。“修改”二字重要，“能在浏览器实时反馈”部分正确✔，应该用到最浪漫的数学用语“能且只能”，因为这里的修改不会影响到源文件；

e.g.
![](https://github.com/TUARAN/pic/blob/master/js/elments改.png)


# 3
### Elment的功能是：“查看已解析的源码HTML中的任一元素，手动修改元素的属性和样式能且只能实时在浏览器里得到反馈”

3.补充：Elment就是最最基础的面板，没什么多的好说的，如果想了解更多？

## [谷歌浏览器开发者工具中文文档](http://www.css88.com/doc/chrome-devtools/inspect-styles/) 关于elments的说明

编辑DOM是在Elemnts比较关键的操作！



