# 背景background综合属性

## 1.背景颜色background-color





## 2.背景图片background-image





## 3.背景重复background-repeat

作用：设置背景图渲染状态

repeat：背景重复渲染，默认

no-repeat：不重复渲染

repeat-x；repeat-y；分别代表水平平铺，垂直平铺



## 4.背景定位background-position

**背景定位**

- ### 4.1单词表示法

- 第一个属性值：left、center、right

- 第二个属性值：top、center、bottom



- ## 4.2像素表示法

以px为单位的数值

- 第一个属性值：表示水平方向

- 第二个属性值：表示垂直方向



- ## 4.3百分比表示法

- 水平方向：100%=（盒子的width）-图片的宽度

- 垂直方向：100%=（盒子的width）-图片的高度



## 5.背景附着background-attachment

作用：设置背景图是否随着页面滚动而滚走

属性值：scrool 				滚动的，默认值，会随页面滚动而滚动

属性值：fixed					固定的，不会随着页面的滚动而滚动



## 6.背景background的综合属性

属性值可以为1-5个





## 背景的应用

### 1、logo替换文案

h1标签通常是制作logo的，目的是为了优化搜索引擎，搜索引擎抓取的是文字而不是logo图片，所以我们可以利用文字和图片制作该效果。

- **原理就是使用背景图片替换文字，文字通过text-indent属性为负值智之后除了h1盒子的显示范围，然后overflow:hideen 隐藏起来，从而实现了logo替换文字**



### 2.利用padding制作背景图

- 例子：**将原来ul的默认小黑点去掉（list-style:none）然后通过li标签的左padding挤出位置，由于背景是可以在padding中加载的，所以给每一个li标签设置背景图片即可**



### 3.精灵

精灵就是和背景定位反向而驰，背景定位都是图片小盒子大，如果此时盒子大，图片小怎么显示？

答：可以利用这种只显示局部的特点制作背景精灵

原理：**如果需要显示某个位置的图片可以利用background-position:- **

背景精灵就是将很多小的icon图标汇集在一起显示，有利于网页加载的速度
