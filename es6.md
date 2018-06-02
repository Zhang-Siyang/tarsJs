1.es6 const:es6 const声明一个只读的常量

2.闭包再解析var/let（作用域 ES5\6）：

ES5：
```javascript
const a=[];
for(var i=0;i<=2;i++){
     a[i]=function(){
        return i*2
     }
}
console.table([
     a[0](),
     a[1](),
     a[2](),
])
```
输出结果：
![](https://github.com/TUARAN/PIC/blob/master/js/bibaotest.png)

注意点：return i*2  

在没被执行时只是一个表达式，所以此时的i一直都是个变量而不是一个值，当进行调用的时候，因为var i=0这里的i是一个全局变量，这里的值已经变成了3，所以，最终执行的是3*2，也就是6了

ES6:
```javascript
const a=[];
for(let i=0;i<=2;i++){
     a[i]=function(){
        return i*2
     }
}
console.table([
     a[0](),
     a[1](),
     a[2](),
])
```
输出结果：
![](https://github.com/TUARAN/PIC/blob/master/js/bibaotest2.png)

