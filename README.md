# Js-
js原生之路

#怎么说呢？JS对于数组的各种操作是很重要的点，却又容易被遗忘的点;

#怎么说呢？JS的闭包！！！闭包！！！吃了2+回的亏了！！！

###1.解析闭包以及基本类型、引用类型（因为弄混过）

闭包：有权访问另一个函数作用域内变量的函数都是闭包。

js的每个函数都是一个个小黑屋，它可以获取外界信息，但是外界却无法直接看到里面的内容。
```javascript
function a(){
  var n = 0;
  function inc() {
    n++;
    console.log(n);
  }
  inc(); 
  inc(); 
}
a(); //控制台输出1，再输出2

function a(){
  var n = 0;
  this.inc = function () {
    n++; 
    console.log(n);
  };
}
var c = new a();
c.inc();  //控制台输出1
c.inc();  //控制台输出2

function a(){
  var n = 0;
  function inc(){
    n++; 
    console.log(n);
  }
  return inc;
}
var c = a();
c();  //控制台输出1 
c();  //控制台输出2
      //注意，函数名只是一个标识（指向函数的指针），而()才是执行函数。
```
将变量 n 放进小黑屋里，除了 inc 函数之外，没有其他办法能接触到变量 n，而且在函数 a 外定义同名的变量 n 也是互不影响的，这就是所谓的增强“封装性”。

`以上摘自“一分钟理解js闭包”`

但是看图说话总是会好一点：

![](https://github.com/TUARAN/PIC/blob/master/js/bibao.png)

```javascript
function f1(){
        var n=9;
        function f2(){
        console.log("wowowowow")
        }
        return f2;     
}
f1();
```

