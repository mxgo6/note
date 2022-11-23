# CSS样式表的使用

使用方法：

- 行内式
- 内嵌式
- 外链式
- 导入式

## 1.行内式样式表

-基本语法

```html
<div style="background:blue;">
    
</div>
```

## 2.内嵌式样式表

-基本语法

写在head中

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>title</title>
    <style>
        div{
            color:blue;
            font-size:20px;
        }
    </style>
</head>
<body>
    <div>文字123</div>
    
</body>
</html>
```

## 3.外链式样式表

-基本语法

从外部引入css文件

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>title</title>
    <link rel="stylesheet" href="css/1.css">
</head>
<body>
    <div>文字123</div>
    
</body>
</html>
```

```css
div{
    color:red;
    font-size:20px;
}
```

## 4.导入式样式表

需要了解！

-基本语法

写在head中，必须写在style标签的最底部用import引入

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>title</title>
    <style>
      @import url(css/1.css);
    </style>
</head>
<body>
    <div>文字123</div>
    
</body>
</html>
```

## 四种样式表的比较

行内式权重最高