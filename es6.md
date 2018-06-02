1.es6 const:es6 const声明一个只读的常量

2.闭包再解析：
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
