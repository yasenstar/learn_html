# HTML学习笔记 2017

[TOC]

HTML 的全称是 Hyper-Text Markup Language （超文本标记语言）

## 什么是 MARKUP LANGUAGE （标记语言）？

``` HTML
<h1>This is a heading</h1>
<p>This is a paragraph of text</p>
```
## 基本的HTML页面

### 最简单的HTML页面

``` html
<!DOCTYPE html>
hello world!!!
```
### 一个HTML页面模板

``` html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        This is the body of the document.
    </body>
</html>
```

# 结构性的文本

``` html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <h1>This is a top level heading</h1>
        <h2>This is a second level heading</h2>
        <h3>This is a third level heading</h3>
    </body>
</html>
```

## 列表 LISTS

## 表格 TABLES

## 表单FORMS

表单是HTML中用来从用户那里获取输入的元素，包括：
* Text Fields（文本框）
* Select Lists （选择列表）
* Text Boxes (多行文本框)
* Checkboxes （复选框）
* Radio Buttons （单选框）
* Password Fields （密码框）

### Text Fields（文本框）

使用两个文本框的示例页面：

``` HTML
<body>
    <form action="submit.html" method="post">
        <label for="firstName">First Name</label>:
        <input id="firstName" name="firstName" type="text"/>
        <p>
        <label for="lastName">Last Name</label>:
        <input id="lastName" name="lastName" type="text"/>
        <p>
        <input type=submit" value="Submit">
    </form>
</body>
```

增加一个文本框的例子：

在之前的contacts.html文件中，增加下面的DIV部分：

``` HTML
<div id="contactDetails"><h2>Contact Details</h2>
    <form method="post">
        <div lass="formRow">
            <label for="contactName">Contact Name</label>
            <input name="contactName" id="contactName" type="text"/>
        </div>
    </form>
</div>
```

为了使各个标签和文本框的风格都一致，在contacts.css中增加如下的风格语句：

``` CSS
label {
    width: 150px;
    display: inline-block;
    vertical-align: top;
}

input {
    width: 200px;
}
```

注意：你需要把label的显示类型做相应改变已适应宽度。

你可以输入如下代码啦：

``` HTML
<div class="formRow">
    <label for="phoneNumber">Phone Number</label>
    <input name="phoneName" id="phoneNumber" type="text"/>
</div>
<div class="formRow">
    <label for="emailAddress">Email Address</label>
    <input name="emailAddress" id="emailAddress" type="text"/>
</div>
```

### Select Lists （选择列表）

输入如下代码以实现单位名称的选择：

``` HTML
<div class="formRow">
    <label for="companyName">Company Name</label>
    <select name="companyName" id="companyName">
        <option value="-1">请选择</option>
        <option value="1">ABC公司</option>
        <option value="2">XYZ公司</option>
        <option value="3">CCC公司</option>
    </select>
</div>
```

注意选择列表是包裹在select的标签中，在这个标签中，可以包含多个选择项option标签来提供不同的可能选择。
每个option有两个值组成：
1. 在option的两个标签中的文字是显示给用户的提示文字；
2. option的value属性是赋值给选择项的值

默认的 ，一个选择列表会选择第一个选择，你可以增加一个布尔值（是、否）来预先指定默认值：

``` HTML
<option value="3" selected>CCC公司</option>
```

### Text Boxes (多行文本框)
### Checkboxes （复选框）
### Radio Buttons （单选框）
### Password Fields （密码框）

## HTML5数据校验

## 拖放

## 动态元素

# CSS

# JAVASCRIPT

