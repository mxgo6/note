# CSS常用属性

## css常用文字属性

有3个：

- color、font-size、font-family

### 1.文字颜色

#### color

- 使用方法

~~~html
<p style="color:blue;">
    看看我的颜色
</p>
~~~

属性值：主要分为两种----**单词表示法**、**颜色值表示法（十六进制，RGBA）**

### 2.字号

#### font-size

~~~html
<p style="font-size:20px;">
    看看我的大小
</p>
~~~

属性值：px为单位的数值

### 3.字体

#### font-family

~~~html
<p style="font-family:'宋体','微软雅黑','Arial','consolas'">
    看看我的字体
</p>
~~~

属性值：双引号包裹，属性值可以有多个，使用逗号隔开(如果不识别前面的字体，就会自动识别后面的字体)

## 盒子的属性

有3个：

- width、height、background-color
> - width：宽度
>
> - height：高度
>
> - background-color：背景颜色
>
>   属性值：px为单位的数值

```html
<div style="width:100px;height:100px;background:red;">
    
</div>
```

## 文本

### **对齐：text-algin**

作用：用来设置段落的整体水平方向对齐

属性值：left、center、right

### **文本修饰text-decoration**

作用：设置文本整体是否有线条修饰

属性值：

- none：没有修饰
- overline：上划线
- line-throught：中划线、删除线
- underline：下划线

### **缩进text-indent**

作用：设置段落首行缩进

属性值：px、em（缩进几个中文字符）、%
