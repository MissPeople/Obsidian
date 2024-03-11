# 1:创建标题：在单词或者短语前加上#号，数量代表级数  
eg:  
# this is first level  
## this is second level  
  
也可在文本下方添加任意数量的==号来标识一级标题，--标识二级标题（不推荐）  
this is first level  
==  
  
## this is second level  
--  
  
# 2:段落  
使用空白行将一行或多行文本进行分隔  
eg:  
this is first line  
  
this is second line  
  
# 3:换行  
在行末添加<br>标签  
eg: I like writing<br>  
  
# 4:强调  
粗体: I like **spring**  
斜体: I like *spring*  
斜体加粗: I like ***spring***  
  
# 5:引用  
在段落前加>可实现引用  
eg:  
> I like spring  
  
# 6:列表  
有序列表:在每个列表项前添加数字并紧跟英文句号，必须以数字1开始，可以不按顺序。  
eg:  
1. I like spring  
2. I like winter  
  
无序列表:在每个列表项前添加-  
eg:  
- I like spring  
- I like winter  
  
要在保留列表连续性的同时在列表中添加另一种元素，将该元素缩进四个空格或一个制表符  
eg:  
* This is the first list item.  
* Here's the second list item.  
  
I need to add another paragraph below the second list item.  
  
* And here's the third list item.  
  
eg:  
* This is the first list item.  
* Here's the second list item.  
  
> A blockquote would look great below the second list item.  
  
* And here's the third list item.

# 7:分割线
在单独一行上使用三个或多个星号 (`***`)、破折号 (`---`) 或下划线 (`___`) ，并且不能包含其他内容
***
---
___

为了兼容性，应在分割线前后都加上空行

***

hello
# 8:链接语法
超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`
eg:
[Markdown语法官网](https://markdown.com.cn)

[Markdown语法官网](https://markdown.com.cn "Markdown教程")

网址和email地址
eg：
<https://markdown.com.cn>

<understandable997@gmail.com>

带格式化的链接
强调链接，在链接前后加上`*`号，要将链接表示为代码，在方括号中添加反引号
eg:
I love the website **[百度](www.baidu.com)**

the url can't click [`baidu`](www.baidu.com)

# 9:图片语法
插入图片Markdown语法代码：`![图片alt](图片链接 "图片title")`。

eg:
![这是图片](https://markdown.com.cn/assets/img/philly-magic-garden.9c0b4415.jpg 复杂)

链接图片
给图片增加链接，将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。
[![这是图片](https://markdown.com.cn/assets/img/philly-magic-garden.9c0b4415.jpg 复杂)](www.baidu.com "去百度看看")


# 10:转义字符语法
要显示原本用于格式化 Markdown 文档的字符，在字符前面添加反斜杠字符 \