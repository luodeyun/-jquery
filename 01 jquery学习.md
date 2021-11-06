### jquery

#### 1.引入jquery

```
    <script src="http://ajax.aspnetcdn.com/ajax/jQuery/jquery-1.8.0.js"></script>(缺点：慢)
```

```js
$(function() {  // 表示页面加载完后再执行函数内容 相当与window.onload
  $('#btnId').click(function(){
    alert('nihao')
  })
})
```

##### 疑问： jquery的$是什么？

##### **答： 其本质就是一个函数，在源码中最后一段：window.$ = jquery**

#### 2.jquery核心函数的4个作用

一.传入参数为函数时，在文档加载完成后执行这个函数

二.传入参数为[HTML字符串]时。根据这个字符串创建元素节点对象

```js
$('<span>1</span>').appendTo('body')
```

三.传入参数[选择器字符串]时

​      $('#id'): id选择器，根据id查询标签对象

​      $('标签名')： 标签选择器，根据指定的标签名查询标签对象

​      $('.class属性值'): 类型选择器 可以根据class查询类标签对象

四.传入参数为[DOM]对象时，将DOM对象包装为jQuery对象返回

### 3.jquery对象和DOM对象的区别

打印不一致

### 4.jquery本质是什么?

jquery对象是dom对象的数组， jquery提供的一系列功能函数

### 5.Dom对象和jquery对象互转

  1.dom对象转化为jQuery对象

​       先有DOM对象在$(DOM对象)就可以转化为jquery对象

   2.jquery对象转化为dom对象

​      先有jquery对象在jquery对象下标去除DOM对象

