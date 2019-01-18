* [vuex](https://segmentfault.com/a/1190000009404727)
* [浅谈vue中慎用style的scoped属性](https://www.jb51.net/article/129228.htm)
* vue请求后台:vue本身不支持发送AJAX请求，需要使用vue-resource（vue1.0版本）、axios（vue2.0版本）等插件实现  [链接](https://www.cnblogs.com/xuanan/p/7847233.html)
```
vue-resourse:

this.$http
  .get(
    'url'
  )
  .then(
    response => {
      console.log('success')
    },
    response => {
      console.error('error')
    }
  )
  
this.$http
  .jsonp(
    'url'
  )
  .then(
    response => {
      console.log('success')
    },
    response => {
      console.error('error')
    }
  )
  
jsonp支持跨域 
```
