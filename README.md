## Bootstrap基础
### Bootstrap简介
#### 基础模板
注意:
- 如果要使用Bootstrap的js插件，必须先调入jQuery
- bootstrap模板为使IE6、7、8版本（IE9以下版本）浏览器兼容html5新增的标签，引入下面代码文件即可。
<script src="https://oss.maxcdn.com/libs/html5shiv/3.7.0/html5shiv.js"></script>

- 同理为使IE6、7、8版本浏览器兼容css3样式，引入下面代码：
<script src="https://oss.maxcdn.com/libs/respond.js/1.4.2/respond.min.js"></script>
```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>Bootstrap的HTML标准模板</title>
	<!-- Bootstrap -->
	<link href="/node_modules/bootstrap/dist/css/bootstrap.min.css" rel="stylesheet">

</head>
<body>
<h1>Hello, world!</h1>

<!-- 如果要使用Bootstrap的js插件，必须先调入jQuery -->
<script src=" /node_modules/jquery/dist/jquery.min.js"></script>
<!-- 包括所有bootstrap的js插件或者可以根据需要使用的js插件调用　-->
<script src="/node_modules/bootstrap/dist/js/bootstrap.min.js"></script>
</body>
</html>
```

#### 全局样式
```html
<!DOCTYPE HTML>
<html>
<head>
	<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
	<title>全局样式</title>
	<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css">
</head>

<body>

<!-- Main jumbotron for a primary marketing message or call to action -->
<div class="jumbotron">
	<h1>Hello, world!</h1>
	<p>This is a template for a simple marketing or informational website. It includes a large callout called a jumbotron and three supporting pieces of content. Use it as a starting point to create something more unique.</p>
	<p><a href="#" >Learn more »</a></p>
</div>

</body>
</html>
```

### 排版
#### 标题(一)
h1~h3的margin为20px；h4-h6的margin为10px
定义了6个类名。h1 h2 h3 h4 h5 h6
大小：h1为36px，依次减6
```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>标题（一）</title>
<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css">
</head>

<body>
<!--Bootstrap中的标题-->
<h1>Bootstrap标题一</h1>
<h2>Bootstrap标题二</h2>
<h3>Bootstrap标题三</h3>
<h4>Bootstrap标题四</h4>
<h5>Bootstrap标题五</h5>
<h6>Bootstrap标题六</h6>

<!--Bootstrap中让非标题元素和标题使用相同的样式-->
<div class="h1">Bootstrap标题一</div>
<div class="h2">Bootstrap标题二</div>
<div class="h3">Bootstrap标题三</div>
<div class="h4">Bootstrap标题四</div>
<div class="h5">Bootstrap标题五</div>
<div class="h6">Bootstrap标题六</div>


</body>
</html>
```
#### 标题(二)
1. small的大小是h1-h3的65%
2. small的大小是h4-h6的75%
3. 在bootstrap.css下h1-h6默认的样式大小是不一样的，所以small乘半分比之后大小不一样
```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>标题（二）</title>
<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css">
</head>

<body>

<!--Bootstrap中使用了<small>标签来制作副标题-->
<h1>Bootstrap标题一<small>我是副标题</small></h1>
<h2>Bootstrap标题二<small>我是副标题</small></h2>
<h3>Bootstrap标题三<small>我是副标题</small></h3>
<h4>Bootstrap标题四<small>我是副标题</small></h4>
<h5>Bootstrap标题五<small>我是副标题</small></h5>
<h6>Bootstrap标题六<small>我是副标题</small></h6>

<!--任务填写处-->

孤儿院无私奉献30年  一曲人性的赞歌
</body>
</html>

```

#### 段落（正文文本）

**class="lead"表强调**
```html
<!DOCTYPE HTML>
<html>
<head>
	<meta charset="utf-8">
	<title>段落（正文文本）</title>
	<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css">
</head>

<body>
<p>超酷的互联网、IT技术免费学习平台，创新的网络一站式学习、实践体验；服务及时贴心，内容专业、有趣易学。专注服务互联网工程师快速成为技术高手！</p>
<p>超酷的互联网、IT技术免费学习平台，创新的网络一站式学习、实践体验；服务及时贴心，内容专业、有趣易学。专注服务互联网工程师快速成为技术高手！</p>

</body>
</html>
```

#### 强调内容
#### 加粗
- strong
可以使用b和strong标签直接让文本加粗
```html
<!DOCTYPE HTML>
<html>
<head>
	<meta charset="utf-8">
	<title>粗体</title>
	<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css">
</head>

<body>
<p>我在学习<strong>Bootstrap</strong>，我要掌握<strong>Bootstrap</strong>的所有知识。</p>
<!--下面是任务部分-->
<p>我是一个段落，这个段落中“强调”一词将会加粗显示。</p>

</body>
</html>
```
#### 斜体

- em
```html
<!DOCTYPE HTML>
<html>
<head>
	<meta charset="utf-8">
	<title>斜体</title>
	<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css">
</head>
<body>
<p>我在<em>亚信</em>一起学习<i>Bootstrap</i>的使用。我一定要学会<i>Bootstrap</i>。</p>
<!--下面是任务部分-->
<p>我正在学习Bootstrap。我发现Bootstrap真的好强大。</p>
</body>
</html>
```

#### 强调相关的类

- .text-muted：提示，使用浅灰色（#999）
- .text-primary：主要，使用蓝色（#428bca）
- .text-success：成功，使用浅绿色(#3c763d)
- .text-info：通知信息，使用浅蓝色（#31708f）
- .text-warning：警告，使用黄色（#8a6d3b）
- .text-danger：危险，使用褐色（#a94442）
```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>强调相关的类</title>
<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css">
</head>

<body>
<div class="text-muted">.text-muted 效果</div>
<div class="text-primary">.text-primary效果</div>
<div class="text-success">.text-success效果</div>
<div class="text-info">.text-info效果</div>
<div class="text-warning">.text-warning效果</div>
<div class="text-danger">.text-danger效果</div>
<!--下面是任务部分-->
<p>我是一段危险信息，请用Bootstrap框架中的危险风格显示</p>
</body>
</html>

```


#### 文本对齐风格

- text-left 居左
- text-center 居中
- text-right 居右
- text-justify 两端对齐
```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>文本对齐风格</title>
<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css">
</head>

<body>
<p class="text-left">我居左</p>
<p class="text-center">我居中</p>
<p class="text-right">我居右</p>
<p class="text-justify">There is clearly a need for CSS to be taken seriously by graphic artists. The Zen Garden aims to excite, inspire, and encourage participation. To begin, view some of the existing designs in the list. Clicking on any one will load the style sheet into this very page. The code remains the same, the only thing that has changed is the external .css file. </p>
<!--下面是任务部分-->
<p>给我加个类，我就向右对齐。</p>


</body>
</html>
```
#### 列表--简介
Bootstrap根据平时的使用情形提供了六种形式的列表：
- 普通列表
- 有序列表
- 去点列表
- 内联列表
- 描述列表
- 水平描述列表

```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>列表--简介</title>
<link rel="stylesheet" href="//netdna.bootstrapcdn.com/bootstrap/3.1.1/css/bootstrap.min.css">
</head>

<body>
<ul>
    <li>无序列表信息1</li>
    <li>无序列表信息2</li>
    <li>无序列表信息3</li>
</ul>
<ol>
    <li>有序列表信息1</li>
    <li>有序列表信息2</li>
    <li>有序列表信息3</li>
</ol>
<dl>
    <dt>定义列表标题</dt>
    <dd>定义列表信息1</dd>
    <dd>定义列表信息2</dd>
</dl>
</body>
</html>
```

#### 列表--无序列表、有序列表

无序列表和有序列表使用方式和我们平时使用的一样（无序列表使用ul，有序列表使用ol标签),可以嵌套。

```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>普通列表、有序列表</title>
<link rel="stylesheet" href="//netdna.bootstrapcdn.com/bootstrap/3.1.1/css/bootstrap.min.css">
</head>

<body>
<h5>普通列表</h5>
<ul>
    <li>列表项目</li>
    <li>列表项目</li>
    <li>列表项目</li>
    <li>列表项目</li>
    <li>列表项目</li>
</ul>
<h5>有序列表</h5>
<ol>
      <li>项目列表一</li>
      <li>项目列表二</li>
      <li>项目列表三</li>
</ol>
<h5>有序列表嵌套</h5>
<ol>
    <li>有序列表</li>
    <li>
    有序列表
        <ol>
        <li>有序列表(2)</li>
        <li>有序列表(2)</li>
        </ol>
    </li>
    <li>有序列表</li>
</ol>
<!--下面是代码任务部分-->

</body>
</html>
```

#### 列表--去点列表
class = "list-unstyled"去除默认列表样式风格
```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>去点列表</title>
<link rel="stylesheet" href="//netdna.bootstrapcdn.com/bootstrap/3.1.1/css/bootstrap.min.css">
</head>
<body>
<!--无序列表去点-->
<ul>
    <li>
    项目列表
        <ul>
        <li>带有项目符号</li>
        <li>带有项目符号</li>
        </ul>
    </li>
    <li>
    项目列表
        <ul class="list-unstyled">
        <li>不带项目符号</li>
        <li>不带项目符号</li>
        </ul>
    </li>
    <li>项目列表</li>
</ul>
<!--有序列表去序号-->
<ol>
    <li>
    项目列表
        <ol>
        <li>带有项目编号</li>
        <li>带有项目编号</li>
        </ol>
    </li>
    <li>
    项目列表
        <ol class="list-unstyled">
        <li>不带项目编号</li>
        <li>不带项目编号</li>
        </ol>
    </li>
    <li>项目列表</li>
</ol>
<!--下面是代码任务部分-->
</body>
</html>
```

#### 列表--内联列表
class="list-inline"垂直列表变成水平列表，实现内联（内敛列表不能改变高度，可以改变宽度）
```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>内联列表</title>
<link rel="stylesheet" href="//netdna.bootstrapcdn.com/bootstrap/3.1.1/css/bootstrap.min.css">
</head>

<body>
<ul class="list-inline">
    <li>W3cplus</li>
    <li>Blog</li>
    <li>CSS3</li>
    <li>jQuery</li>
    <li>PHP</li>
</ul>
<!--下面是代码任务部分-->



</body>
</html>
```

#### 列表--定义列表

- dl 定义列表
- dt 定义列表组
- dd 自定义列表描述

```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>定义列表</title>
<link rel="stylesheet" href="//netdna.bootstrapcdn.com/bootstrap/3.1.1/css/bootstrap.min.css">
</head>

<body>
<dl>
    <dt>W3cplus</dt>
    <dd>一个致力于推广国内前端行业的技术博客</dd>
    <dt>慕课网</dt>
    <dd>一个真心在做教育的网站</dd>
</dl>
<!--下面是代码任务部分-->
</body>
</html>
```

#### 列表--水平定义列表

水平定义列表就像内联列表一样，Bootstrap可以给<dl>添加类名“.dl-horizontal”给定义列表实现水平显示效果。

```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>水平定义列表</title>
<link rel="stylesheet" href="//netdna.bootstrapcdn.com/bootstrap/3.1.1/css/bootstrap.min.css">
</head>

<body>
<dl class="dl-horizontal">
    <dt>W3cplus</dt>
    <dd>技术博客</dd>
    <dt>杨正友</dt>
    <dd>一个专业的，真心实意在做培训的网站</dd>
    <dt>我来测试一个标题，我来测试一个标题</dt>
    <dd>我在写一个水平定义列表的效果，我在写一个水平定义列表的效果</dd>
</dl>
</body>
</html>
```

#### 代码
1. 使用**code**来显示单行内联代码,一般是针对于单个单词或单个句子的代码
2. 使用**pre**来显示多行块代码,一般是针对于多行代码（也就是成块的代码）
3. 使用**kbd**来显示用户输入代码,一般是表示用户要通过键盘输入的内容
4. **pre:** preformatted text
5. **kbd:** keyboard
```html
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>代码</title>
<link rel="stylesheet" href="//netdna.bootstrapcdn.com/bootstrap/3.1.1/css/bootstrap.min.css">
</head>
<body>
code风格：
<div>Bootstrap的代码风格有三种：<code>&lt;code&gt;</code>、<code>&lt;pre&gt;</code>和<code>&lt;kbd&gt;</code></div>
pre风格：
<div>
<pre>
&lt;ul&gt;
&lt;li&gt;...&lt;/li&gt;
&lt;li&gt;...&lt;/li&gt;
&lt;li&gt;...&lt;/li&gt;
&lt;/ul&gt;
</pre>
</div>
kbd风格：
<div>请输入<kbd>ctrl+c</kbd>来复制代码，然后使用<kbd>ctrl+v</kbd>来粘贴代码</div>
<p>请使用ctrl+x复制代码，然后使用ctrl+shift+v将复制的代码粘贴到需要的地方。</p>
</body>
</html>
```