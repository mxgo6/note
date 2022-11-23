# 盒模型

CSS重要布局属性，包含了五个属性：**width(宽度)、height(高度)、padding(内边距)、broder(边框)、margin(外边距)**

盒子的实际加载区域：width+height

盒子可实体化显示区域：width+height+padding+border

盒子实际占位区域：width+height+padding+border+margin



## 1.宽度和高度width、height

注意：如果盒子不设置宽度，会默认铺满父盒子的宽度

​			如果盒子不设置高度，会默认被内容文字撑高

## 2.内边距padding

作用：设置宽到高到边框的间距

特点：不加载内容，但是可以加载背景

padding是一个综合属性，可以根据不同方向进行单一属性的设置

比如padding-left（左边的内边距）、padding-right（右边内边距）、padding-top（上面内边距）、padding-bottom（下面内边距）

还可以写成：

四值法：padding:10px 20px 30px 40px;（上、右、下、左）

三值法：padding:10px 20px 30px;（上、左右、下）

二值法：padding:10px 20px;（上下、左右）

单值法：padding:10px（上下左右）

## 3.边框border

border是一个综合属性，有三个属性值，可以进行单一属性设置

border-width（边框宽度）

border-style（线形）

border-color（线的颜色）



- ### border-width







- ### border-style

> solid：实线
>
> dashed：虚线
>
> dotted：点线
>
> double：双线
>
> groove：边框凹陷效果
>
> rideg：边框凸显效果
>
> inset：内容凹陷效果
>
> outset：内容突出效果



- ### border-color





## 外边距margin

作用：设置盒子与其他盒子之间的间距

写法和padding内边距一样





## 盒模型扩展

### 1.清楚默认样式

### 2.height属性扩展

- overflow:visible作用是：可见的，默认的
- overflow:hidden作用是：超出高度部分，隐藏
- overflow:scroll作用是：给盒子添加滚动条样式
- overflow:auto作用是：盒子超出部分滚动条显示

### 3.居中

- 单行文字：

水平居中：text-align:center

垂直居中：设置line-height的高度和盒子一样高

- 多行文字

垂直居中：盒子不设置高度，设置上下相同的padding

#### 盒子居中

盒子的水平居中：margin:(自定义值) auto

盒子的垂直居中：父盒子高度不设置，而设置上下padding



- 总结：如果设置盒子上下左右都居中的状态，首先盒子设置margin: 0 auto；父盒子不设置高度，而设置上下padding

### 4.margin塌陷现象

同方向的margin会有塌陷（上下）

在垂直方向上，如果有相遇的margin，两个盒子之间不是属性值的和，而是比较两个盒子谁的margin更大，谁的值更大就使用谁的margin
