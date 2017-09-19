---
title: DIV的四种居中方式
date: 2017-07-21 9:52:00
categories: 前端技术栈
tags: html+css
---
> 因为之前面试的时候经常被问到这个问题，在之后的开发阶段也或多或少有接触到DIV的居中情况，所以在这里总结一下，记录下来。[demo](http://zhengcheng.club/demo/center.html)

<br>

#### #demo1
``` bush
    <div id="div1">
        demo1
        <div class="div1"></div>
    </div>

    <style>
        #div1{
            width: 400px;
            height: 400px;
            border: 1px solid #000;
            position: relative;
        }
        .div1{
            width: 100px;
            height: 100px;
            border: 1px solid #ccc;
            background: #99f;
            position: absolute;
            left: 50%;
            top: 50%;
            transform: translate(-50%,-50%);
        }
    </style>
```

#### #demo2
``` bush
    <div id="div2">
        demo2
        <div class="div2"></div>
    </div>

    <style>
        #div2{
            width: 400px;
            height: 400px;
            border: 1px solid #000;
            position: relative;
        }
        .div2{
            width: 100px;
            height: 100px;
            border: 1px solid #ccc;
            background: #f99;
            position: absolute;
            top: 0;
            right: 0;
            bottom: 0;
            left: 0;
            margin: auto;
        }
    </style>
```

#### #demo3
```bush
    <div id="div3">
        demo3
        <div class="div3"></div>
    </div>

    <style>
        #div3{
            width: 400px;
            height: 400px;
            border: 1px solid #000;
            position: relative;
        }
        .div3{
            width: 100px;
            height: 100px;
            border: 1px solid #ccc;
            background: #009688;
            position: absolute;
            left: 50%;
            top: 50%;
            margin-left: -50px;
            margin-top: -50px;
        }
    </style>
```

#### #demo4
``` bush
    <div id="div4">
        <!--demo4-->
        <div class="div4"></div>
    </div>

    <style>
        #div4{
            width: 400px;
            height: 400px;
            border: 1px solid #000;
            display: table-cell;
            vertical-align: middle;
        }
        .div4{
            width: 100px;
            height: 100px;
            border: 1px solid #ccc;
            background: #FF9800;
            margin: auto;
        }
    </style>

```