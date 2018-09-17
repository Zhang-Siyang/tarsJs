# 1
# 2
1.对 new Date()得到的日期进行格式化显示扩展，扩展方法如下：
```
Date.prototype.Format = function (fmt) { //author: meizz 

         var o = {
             "M+": this.getMonth() + 1, //月份 
             "d+": this.getDate(), //日 
             "h+": this.getHours(), //小时 
             "m+": this.getMinutes(), //分 
             "s+": this.getSeconds(), //秒 
             "q+": Math.floor((this.getMonth() + 3) / 3), //季度 
             "S": this.getMilliseconds() //毫秒 
         };
         if (/(y+)/.test(fmt)) fmt = fmt.replace(RegExp.$1, (this.getFullYear() + "").substr(4 - RegExp.$1.length));
         for (var k in o)
             if (new RegExp("(" + k + ")").test(fmt)) fmt = fmt.replace(RegExp.$1, (RegExp.$1.length == 1) ? (o[k]) : (("00" + o[k]).substr(("" + o[k]).length)));
         return fmt;}
```

测试：

```
 (new Date()).Format("yyyy-MM-dd hh:mm:ss.S") //输出结果： 2017-01-23 09:36:10.400
 (new Date()).Format("yyyy-M-d h:m:s.S")      //输出结果： 2017-1-23 9:36:35.572
```
2.计算时间差：
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
