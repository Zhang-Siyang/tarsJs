1.去重：
---
方法一：
new Set(["a","b","b"]); 结果：{"a","b"},将数组去重后的到的是一个对象；
```大家都在发大家都在发大家都在发
var s = new Set(["a", "b","b"]);
Array.from(s);   
(2) ["a", "b"]0: "a"1: "b"length: 2__proto__: Array(0)
```
方法二：
如果有相同的值则跳过，不相同则push进数组;（倒）
```
Array.prototype.distinct = function(){
 var arr = this,
  result = [],
  i,
  j,
  len = arr.length;
 for(i = 0; i < len; i++){
  for(j = i + 1; j < len; j++){//从i+1项开始；
   if(arr[i] === arr[j]){
    j = ++i;
   }
  }//内循环
  console.log(i);
  result.push(arr[i]);
 }//外循环
 return result;
}//当i=0时，当a[0]==a[5]的时候，此时i=1,j=1;继续执行内循环，j++，j=2，继续判断,  
             //当到a[1]和a[7]相等时，i=2,j=2;继续执行内循环，j++,j=3,继续判断，
             //当到a[2]没有和a[x]相等时，当a[2]时，没有相等的元素和它再相等，跳出内循环，执行外循环，则push a[2]
             //然后a++,a=3,再到内循环；
             //a[3]=a[4]时，a=4,j=4;继续执行内循环，j++,j=5，继续判断，
             //a[4]没有和a[x]相等时，当a[2]时，没有相等的元素和它再相等，跳出内循环，执行外循环，则push a[4]
             //然后a++,a=5,再到内循环；
             //......
             //总结:怎么判断这个数是唯一的呢，就是它后面没有数跟它一样了，如果它后面还有数跟它一样，就直接“扔掉它”，push最后的是唯一的那个就好了，
             //所以最后的结果[3,4,2,1]就是[a[2],a[4],a[7],a[10]]
var arra = [1,2,3,4,4,1,1,2,1,1,1]; 
arra.distinct();    //返回[3,4,2,1]
```
2.Array对象属性：
---
[菜鸟教程：为什么要叫菜鸟教程呢？因为如果连这些还不熟悉，的确挺菜鸟的](http://www.runoob.com/jsref/jsref-obj-array.html)

3.Array对象属性：join():/reverse():/        (面试题“回文”经常出现！)
---
```
var a=["tom","john","ted"]
console.log(a.join());//tom,john,ted  将数组转化成字符串；
console.log(a.join("."))//tom.john.ted
console.log(a.join(""))//tomjohnted
```
```
var b=["tt","gg","oo"]
console.log(b.reverse());//["oo", "gg", "tt"] 数组倒序
```
4.Array对象属性敲重点：
---
concat()	连接两个或更多的数组，并返回结果。

fill()	使用一个固定值来填充数组。

filter()	检测数值元素，并返回符合条件所有元素的数组。

find()	返回符合传入测试（函数）条件的数组元素。


forEach()	数组每个元素都执行一次回调函数。

from()	通过给定的对象中创建一个数组。

indexOf()	搜索数组中的元素，并返回它所在的位置。

isArray()	判断对象是否为数组。

join()	把数组的所有元素放入一个字符串。

map()	通过指定函数处理数组的每个元素，并返回处理后的数组。

pop()	删除数组的最后一个元素并返回删除的元素。

push()	向数组的末尾添加一个或更多元素，并返回新的长度。

reduce()	将数组元素计算为一个值（从左到右）。

reverse()	反转数组的元素顺序。

shift()	删除并返回数组的第一个元素。

slice()	选取数组的的一部分，并返回一个新数组。

sort()	对数组的元素进行排序。

splice()	从数组中添加或删除元素。

toString()	把数组转换为字符串，并返回结果。

unshift()	向数组的开头添加一个或更多元素，并返回新的长度。

valueOf()	返回数组对象的原始值。

# 5.两个Array数组中是否有重复的值
```
Array.ExistsSameValues = function(a1, a2) {
    var exists = false;
    if(a1 instanceof Array && a2 instanceof Array)
    {
        for (var i=0,iLen=a1.length; i<iLen; i++)
        {
            for (var j=0,jLen=a2.length; j<jLen; j++)
            {
                if (a1[i]===a2[j])
                {
                   console.log(a1[i]);
                }
            }
        }
    }
    return exists;
};
 
var a1 = [1, 2, 5, 8];
var a2 = [3, 1, 9, 5];
Array.ExistsSameValues(a1, a2);
```


