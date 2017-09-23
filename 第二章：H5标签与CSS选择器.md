# 第二章：H5标签与CSS选择器

标签（空格分隔）： html

---


2.1 - a标签/span标签
----------------

2.1.1 - **a标签四个伪类**

    a:link {color: #FF0000;}          /* 未访问的链接 */
    a:visited {color: #00FF00;}	/* 已访问的链接 */
    a:hover {color: #FF00FF;}     /* 鼠标移动到链接上 */
    a:active {color: #0000FF;}	/* 选定的链接 */

a:link,a:visited,a:hover,a:active,错误的顺序有时会使超链接的样式失效；
2.1.2 - span标签

2.2 - 常用标签
----------

2.2.1 - 常用标签：h1-h6、p、strong、em、span、ul、ol、li、dl、dt、dd
2.2.2 - HTML5新增标签：header、nav、footer、section、article、aside、time、mark…
2.3 - 特殊的img

2.4 - 常用选择器
-----------

2.4.1 - **id选择器**
id是元素的唯一标识符，不可出现重复的id名；
id选择符的语法格式是“#”加上自定义的id名
      如：#box{width:300px; height:300px;}

2.4.2 - **类选择器**
类选择符的语法格式：
    

    如：<div class="top"></div>
               .top{属性:属性值;}

2.4.3 - **标签选择器**
2.4.4 - **群组选择、包含选择器**
2.4.5 - **通配符**

    语法：*{属性：属性值;}    常用来重置样式

2.5 - 选择器优先级
------------

2.5.1 - 基础选择器优先级
style>id>class>类型选择>*
2.5.2 - 包含选择器优先级计算
2.5.3 - 群组选择器优先级
 div+p会选中离div最近的兄弟元素p;

2.6 - css reset
---------------

    body,dl,dd,p,h1,h2,h3,h4,h5,h6{
        margin:0;font-size:12px;
    }
    ol,ul{
        margin:0;
        padding:0;
        list-style:none;
    }
    a{
        text-decoration:none;
    }
    img{
        border:none;
        vertical-align :top;
    }

2.7 - 块元素及特征
------------

1、默认独占一行
	2、没有宽度时，默认撑满父级的宽度
	3、支持所有css命令

2.8 - 内联元素及特征
-------------

1、同排可以继续跟同类的标签
	2、内容撑开宽度
	3、不支持宽高
	4、不支持上下的margin
	5、代码换行被解析

2.9 - 块与内联的转换
2.10 - inline-block
2.10.1 - inline-block的特性
特性：
1、块在一行显示；
2、行内属性标签支持宽高；
3、没有宽度的时候内容撑开宽度

问题：
1、代码换行被解析；
2、ie6 ie7 不支持块属性标签的inline-block;

2.10.2 - inline-block的问题
2.11 - vertival-align

前端规范
----

1、所有书写均在英文半角状态下的小写；
2、id，class必须以字母开头；
3、所有标签必须闭合；
4、html标签用tab键缩进；
5、属性值必须带引号；
6、<!-- html注释 -->
7、/* css注释 */
8、ul,li/ol,li/dl,dt,dd拥有父子级关系的标签；
9、p,dt,h标签  里面不能嵌套块属性标签；
10、a标签不能嵌套a；
11、内联标签不能嵌套块标签；







