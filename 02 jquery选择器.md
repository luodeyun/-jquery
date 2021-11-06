

#### 基础选择器与之前的一样 如 id 标签， class *

#### 现在看一下层级选择器

1. 含义： 在给定的祖先元素下匹配所有的后代元素

#####        $('form input') 表示查找form表单中查找input元素

#####        $('form > input ')表示查找from表单中所有子级input元素

#####        $ ('lable + input')表示匹配所有紧接着prev元素后的next元素(匹配一个)

#####        $('lable ~ input')表示prev元素之后的所有兄弟元素（匹配多个）

2. 过滤选择器

   $('li : first') 获取匹配的第一个元素

   $('li : last') 获取匹配的最后一个元素

​        $('li : even') 获取匹配的偶数元素

​        $('li : odd') 获取匹配的奇数元素

​        $('li : gt(0)') 获取匹配的下标大于0的元素

​         $('li : lt(0)') 获取匹配的下标小于0的元素

   3.内容过滤器

​         $('div:contains('John)')包含给定文本的元素

​         $('div:empty')查找所有不包含子元素或者文本的空元素

​         $('div:parent')查找所有包含子元素或者文本的空元素

​         $("div:has(p)")查找div中包含p标签的元素返回div标签

​    4.属性选择器

​           $('div[name]')查找div中包含name的属性

​            $('div[name =value]')查找div中包含name的值为value的属性            

​            $('div[name !=value]')查找div中包含name的值不为value的属性    

​            $('div[name ^=va]')查找div中包含name的值为va开头的属性    

​            $('div[name$=va]')查找div中包含name的值为va结尾的属性    

​      5.表单对象属性选择器

​           $(':input')查找表单中input值

​          以此类推 password checked 的type类型

获取input的值我们可以使用val 

val()可以操作**表单项**的vakue属性值，

他可以设置和获取

$(':text:enabled').val('万能丑小鸭') 

each方法是jquery对象提供用来遍历元素的方法

在遍历的function函数中，有个this对象，这个this对象，js当前遍历的dom对象

