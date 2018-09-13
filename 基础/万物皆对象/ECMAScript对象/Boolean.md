1.String[对象方法]（http://www.runoob.com/jsref/jsref-obj-string.html）
---
2.String对象方法之split()：把字符串分割为字符串数组；
---
```
var str="How are you doing today?";
console.log(str.split(" "));//["How", "are", "you", "doing", "today?"]
console.log(str.split());//["How are you doing today?"]
console.log(str.split(""))// ["H", "o", "w", " ", "a", "r", "e", " ", "y", "o", "u", " ", "d", "o", "i", "n", "g", " ", "t", "o", "d", "a", "y", "?"]
```
回文：
```
function checkPalindrom(str) {  
    return str == str.split('').reverse().join('');//字符串变数组，再倒序，再变成数组；
}
```
