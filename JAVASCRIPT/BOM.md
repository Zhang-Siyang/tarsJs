# 1
计算时间差：
```
var a=(new Date()).getTime();
var b=(new Date("2018/8/23 23:59:59")).getTime();

console.warn(b-a);//总毫秒数
var d=(b-a)%(1000*3600*24);//天数之后的毫秒数
var e=d%(1000*3600);//小时之后的毫秒数
var f=e%(1000*60);//分钟之后的毫秒数

console.log(Math.floor((b-a)/(1000*3600*24)));//天
console.log(Math.floor(d/(3600*1000)));//小时
console.log(Math.floor(e/(1000*60)));//分钟
console.log(Math.floor(f/1000))//秒
```
