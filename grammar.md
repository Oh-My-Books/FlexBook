# 语法文档

## 容器属性
>在容器上定义子元素的排列方向对齐方式等

- `flex-direction` 排列方向
- `flex-wrap` 如何换行
- `flex-flow` 是flex-direction属性和flex-wrap属性的简写形式
- `justify-content` 对齐方式
- `align-items` 定义子元素在交叉轴上如何对齐
- `align-content` 定义了多根轴线的对齐方式

### `flex-direction` 

#### 说明
- 属性决定主轴的方向（即子元素的排列方向

#### 属性
- `row` 主轴为水平方向，起点在左端
- `row-reverse` 主轴为水平方向，起点在右端
- `column` 主轴为垂直方向，起点在上沿
- `column-reverse` 主轴为垂直方向，起点在下沿

#### 演示
````html:120
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>flex-direction</title>
    <style>
        .flex-container {
            display: flex;
            flex-direction: row;  /* 默认 */
        }
        .item{
            display: inherit;
            width:100px;
            height:100px;
            align-items: center;
        }
        .item p{
            width:100%;
            text-align:center;
            color:#fff;
        }
    </style>
</head>
<body>

<div class="flex-container" id="direction">
    <div class="item" style="background-color: #2a80b9;"><p>1</p></div>
    <div class="item" style="background-color: #8f44ad;"><p>2</p></div>
    <div class="item" style="background-color: #16a086;"><p>3</p></div>
    <div class="item" style="background-color: #f1c40f;"><p>4</p></div>
    <div class="item" style="background-color: #e77e23;"><p>5</p></div>
</div>
</body>
</html>
````

### `flex-wrap` 
### `flex-flow` 
### `justify-content` 
### `align-items` 
### `align-content` 

## 子元素属性
- `order` 元素排列顺序
- `flex-grow` 定义子元素的放大比例
- `flex-shrink` 定义了子元素的缩小比例
- `flex-basis` 定义了在分配多余空间之前，子元素占据的主轴空间
- `flex` 是flex-grow, flex-shrink 和 flex-basis的简写
- `align-self` 允许单个子元素有与其他子元素不一样的对齐方式
