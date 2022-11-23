# CSS选择器

分为两种：

**基础选择器**：标签选择器、id选择器、类名选择器

**高级选择器**：后代选择器、交集选择器、并集选择器

## 1-1.标签选择器

选择方法：标签名

选择范围：HTML中所有的同名标签

```html
<head>
<style>
p{
	color:red;
}
div{
	color:blue;
}
</style>
</head>
<body>
    <p>
        p
    </p>
    <div>
        div
    </div>
</body>

```

## 1-2.id选择器

选择方法：通过标签的id属性选择

书写方法：#id

选择范围：一个id标签

```html
<head>
<style>
# p1{
	color:red;
}
</style>
</head>
<body>
<p id="p1">
    第一段文字
</p>
<p>
    第二段文字
</p>
</body>
```

id属性具有唯一性

优点：权重高

## 1-3.类名选择器

选择方法：通过标签上的class属性进行选择

书写方法：.匹配对应class属性值

选择范围：选择所有同名class属性标签

```html
<head>
<style>
.p1{
	color:red;
}
</style>
</head>

<body>
    <p class="p1">
    第一段文字
</p>
<p>
    第二段文字
</p>
</body>

```

class值可以设置一个或多个

class属性命名规范：由字母、数字、下划线组成，且第一个字符必须是字母。

## 1-4.通配选择器

书写方法：*

选择范围：选中包含html标签在内的所有标签

通配符*后面添加的样式，每一个标签都会加在一次

我们通常使用清除页面的默认样式

```html
<head>
<style>
*{
	color:red;
}
</style>
</head>

<body>
    <p>段落</p>
    <span>span</span>
    <div>div</div>
</body>

```

**清除页面默认的内外边距**

```html
*{
	margin:0;
	padding:0;
}
```

## 2-1.后代选择器

通过标签之间的后代关系去决定选择某个范围内的元素

书写方法：使用空格连续链接多级选择器

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .box ul li {
            color:red;
        }
        .box2 ul li {
            color:blue;
        }
    </style>
</head>
<body>
    <div class="box">
        <ul>
            <li>box里面的li</li>
            <li>box里面的li</li>
            <li>box里面的li</li>
            <li>box里面的li</li>
        </ul>
    </div>
    <div class="box2">
        <ul>
            <li>box2里面的li</li>
            <li>box2里面的li</li>
            <li>box2里面的li</li>
            <li>box2里面的li</li>
        </ul>
    </div>
</body>
</html>
```

需要注意的是，后代关系不一定是父子关系

## 2-2.交集选择器

将满足所有选择器条件的匹配

书写方法：将多个选择器链接书写，中间不需要加符号
