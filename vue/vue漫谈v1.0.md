#### V1.0

😂vue看过基本一遍后，请前往学习vue-cli，了解vue-cli搭建vue项目特别重要：http://www.jb51.net/article/111658.htm ！
***
👂从Jquery中脱离出来学习vue，可以试图理解以下demo：

```javascript
<body>
    <div id="app">
        <ul>
            <!--根据数组数据自动渲染页面-->
            <li v-for="item in message">{{item}}</li>
        </ul>
        <button @click="add">添加数据</button>
    </div>
    <div id="app1">
        <ul id="list">
            <li>第1条数据</li>
            <li>第2条数据</li>
        </ul>
        <button id="add">添加数据</button>
    </div>
</body>

<script src="https://unpkg.com/vue/dist/vue.js"></script>
<script>
    new Vue({
        el: '#app',
        data: {
            message: ["第1条数据", "第2条数据"],
            i: 2
        },
        methods: {
            //向数组添加一条数据即可
            add: function() {
                this.i++
                this.message.push("第" + this.i + "条数据")
            }
        }
    })
</script>


<script src="https://cdn.bootcss.com/jquery/3.2.1/jquery.min.js"></script>
<script>
    $(document).ready(function() {
        var i = 2;
        $('#add').click(function() {
            i++;
            //通过dom操作在最后一个li元素后手动添加一个标签
            $("#list").children("li").last().append("<li>第" + i + "条数据</li>")
        });
    }); 
</script>

```
***
🌂Vue的重点有：数据双向绑定、生命周期、多页面Vue、Vue的组件化思想等!
***
👹这里以一个很重要的组件例子作为说明，一些vue封装的组件例如[Elment Table](http://element.eleme.io/#/zh-CN/component/table)组件:
[vue组件化构建](https://cn.vuejs.org/v2/guide/#组件化应用构建);
***
🌫Prop:（单项数据流 父传子）

*父
```javascript
<template>
  <div id="app">
    <tarbtn :msg="message"></tarbtn>
  </div>
</template>

<script>
import Tarbtn from "@/components/Tarbtn.vue";
export default {
  components:{
    Tarbtn:Tarbtn,
  },
  name: 'App',
  data(){
    return{
       message: 'hello props'
    }
  }
}
</script>
```
*子
```javascript
<template>
  <div>
      <p>{{ msg }}</p>
  </div>
</template>

<script>
export default {
  props: ['msg'],
}
</script>
```
***
🐻Vue深入响应式原理(从nextTick看)：

虽然 Vue.js 通常鼓励开发人员沿着“数据驱动”的方式思考，避免直接接触 DOM，但是有时我们确实要这么做。为了在数据变化之后等待 Vue 完成更新 DOM ，可以在数据变化之后立即使用 Vue.nextTick(callback)。这样回调函数在 DOM 更新完成后就会调用。

demo:

```javascript
<template>
  <div>
      <div ref="msgDiv">{{msg}}</div>
            <div v-if="msg1">msg1: {{msg1}}</div>
            <div v-if="msg2">msg2 inside $nextTick: {{msg2}}</div>
            <div v-if="msg3">msg3 outside $nextTick: {{msg3}}</div>
            <button @click="changeMsg">
                Change the Message
            </button>
  </div>
</template>
<script>
export default {
  data () {
    return {
    msg: '我是msg的初始值',
    msg1: '我是msg1',
    msg2: '我是msg2',
    msg3: '我是msg3',
    };
  },
  methods: {
    changeMsg() {
      this.msg = "我是点击btn后改变的msg的值"

      this.msg1 = this.$refs.msgDiv.innerHTML
      this.$nextTick(() => {
        this.msg2 = this.$refs.msgDiv.innerHTML
      })
      this.msg3 = this.$refs.msgDiv.innerHTML
    }

 }
}
</script>
```
结果：

![](https://github.com/TUARAN/tarsVue1.0/blob/master/nextTick0.png) 

![](https://github.com/TUARAN/tarsVue1.0/blob/master/nextTick1.png) 

比较[nextTick和$nextTick](http://www.flowerboys.cn/VueJs/2017/0614/99.html)
***
😜说到通信不可避免的就是[EventBus和VueX](https://segmentfault.com/a/1190000008184629)了

EventBus:

1.创建：发送端和接收端引入
```javascript
import Bus from 'common/js/bus.js';
```
2.发送端：
```javascript
 Bus.$emit('getTarget', event.target);
```
3.接收端：
```javascript
Bus.$on('getTarget', target => {  
            console.log(target);  
        });  
```
vueX:

[vuex github](https://github.com/vuejs/vuex)

![](https://github.com/TUARAN/PIC/blob/master/common/vuex.png)
