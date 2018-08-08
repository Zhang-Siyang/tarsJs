![缓存](https://github.com/TUARAN/pic/blob/master/common/缓存.png)

[sessionId](http://www.cnblogs.com/japanbbq/archive/2011/09/01/2161650.html)

[Session是通过利用设置在Cookie中的id来区分访问的用户](https://blog.csdn.net/s_clifftop/article/details/72854085)

>Cookie如果不设置过期时间（使用setMaxAge()方法），则表示这个cookie生命周期为浏览器会话期间，只要关闭浏览器窗口，cookie就消失了。这种生命期为浏览会话期的cookie被称为*会话cookie*。会话cookie一般不保存在硬盘上而是保存在内存里。 
如果设置了过期时间，浏览器就会把cookie保存到硬盘上，关闭后再次打开浏览器，这些cookie依然有效直到超过设定的过期时间。存储在硬盘上的cookie可以在不同的浏览器进程间共享，比如两个IE窗口。而对于保存在内存的cookie，不同的浏览器还有不同的处理方式。这种Cookie称为*持久Cookie*
