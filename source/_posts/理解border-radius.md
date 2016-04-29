---
title: 利用border-radius画一个鸡蛋
date: 2016-04-27 13:05:33
tags: css
---

`border-radius` 是`css3` 的一个新的特性。一般是用来做圆角的, 但是可以利用它做出很多奇妙的东西， 比如下面这个：

`html`:
``` html
  <div class="egg"></div>
```

`css`:
```css
  .egg {
    width: 126px;
    height: 180px;
    background-color: red;
    border-radius: 50% / 60% 60% 40% 40%
  }
```
[看demo点击这里](jackpanyj.github.io/blog_demo/border-radius/index.html)

解释一下上面的`border-radius`的属性值：

  + `border-radius` 如果少于四个值， 其表示的含义与`margin`， `padding` 类似
  + `border-radius` 如果超过四个值， 用`/`分隔开来， 前面表示水平半径，后面表示垂直半径
利用这个特性， 把一个矩形各个圆角的垂直半径设置为`50%`，讲上面俩个圆角的垂直半径设置为`60%`， 下面俩个圆角的垂直半径设置为`40%` 就实现了用css画鸡蛋的效果
