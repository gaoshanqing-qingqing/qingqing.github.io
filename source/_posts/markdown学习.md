---
title: markdown学习
date: 2024-10-24 17:48:10
tags: 
- markdown
categories: 学习笔记
---

[TOC]

# markdown初级

        我展示的是一级标题
        =
        我展示的是二级标题
        -
我展示的是一级标题
=
我展示的是二级标题
-

总结：
在文字下方一行写1 or n个等于号表示一级标题
在文字下方一行写1 or n个减号号表示二级标题


        # 一级标题
        ## 二级标题
        ### 三级标题
        #### 四级标题
        ##### 五级标题
        ###### 六级标题
        #######

# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
####### 不支持七级标题



总结：一共只有六级标题
## markdown的段落格式
### 段落
开启新的段落的两种方式  
后面加上两个空格然后回车（enter）
or空一行
这样的

### 字体

        *斜体文本*
        _斜体文本_
        **粗体文本**
        __粗体文本__
        ***粗斜体文本***
        ___粗斜体文本___

        ###分割线
        ***

*斜体文本*  
_斜体文本_  
**粗体文本**  
__粗体文本__  
***粗斜体文本***  
___粗斜体文本___  

### 分割线
        ****

        *     *      *
		***

        - - -

        ----------
        *
        **

***

*     *      *

*****

- - -

----------
\*  
**  
总结：3 or n(n>=3)

### 删除线
			RUNOOB.COM
			GOOGLE.COM
			~~BAIDU.COM~~  
  
RUNOOB.COM  
GOOGLE.COM 
~~BAIDU.COM~~    

总结：飘号键盘数字1的左边

### 下划线
		<u>下划线文本</u>
<u>下划线文本</u>

### 脚注

        创建脚注格式类似这样 [^RUNOOB]。

        [^RUNOOB]: 菜鸟教程 -- 学的不仅是技术，更是梦想！！！


创建脚注格式类似这样 [^RUNOOB]。

[^RUNOOB]: 菜鸟教程 -- 学的不仅是技术，更是梦想！！！

总结：脚注对文本的补充说明。

## MarkDown锚点的使用

        MarkDown不支持锚点，所以只能借助html的锚点有两种方式
        <a id="jump1">标题</a>
        <span id="jump2">标题二</span>

        [标题](#jump1)
        [标题二](#jump2)

MarkDown不支持锚点，所以只能借助html的锚点有两种方式  
<a id="jump1" href="#aa">标题</a>  
<span id="jump2">标题二</span>  

<span id="aa">[标题](#jump1)</span>  
[标题二](#jump2)  

总结：标题必须添加a标签或者span标签才行而且必须指定id

## MarkDown插入视频  
html的Iframe标签，可以参考[w3c](https://www.w3school.com.cn/tags/tag_iframe.asp)或者[码农教程](http://www.manongjc.com/html/html_iframe.html)
兼容性不是很好

        <iframe src="http://www.manongjc.com/" width="400" height="400" scrolling="yes" />

        <iframe src="//player.bilibili.com/player.html?aid=684723947&bvid=BV1vU4y1971F&cid=735989487&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

        <video controls height='100%' width='100%' preload="none" poster="http://media.w3.org/2010/05/sintel/poster.png" src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/OpenBrowser.mp4"></video>



<video controls height='100%' width='100%' preload="none" poster="http://media.w3.org/2010/05/sintel/poster.png" src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/OpenBrowser.mp4"></video>



## MarkDown列表
Markdown 支持有序列表和无序列表。

无序列表使用星号(*)、加号(+)或是减号(-)作为列表标记，这些标记后面要添加一个空格，然后再填写内容：

    * 第一项
    * 第二项
    * 第三项

    + 第一项
    + 第二项
    + 第三项

    - 第一项
    - 第二项
    - 第三项

    * 第一项
    * 第二项
    * 第三项


- 第一项
- 第二项
- 第三项

* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项


- 第一项
- 第二项
- 第三项

有序列表使用数字并加上 . 号来表示，如：

    1. 第一项
    2. 第二项
    3. 第三项

1. 第一项
2. 第二项
3. 第三项

## 列表嵌套

      1. 第一项：
          - 第一项嵌套的第一个元素
          + 第一项嵌套的第二个元素
          * 第一项嵌套的第三个元素

      2. 第二项：
          - 第二项嵌套的第一个元素
          - 第二项嵌套的第二个元素
      * 要有缩进 

1. 第一项：
    - 第一项嵌套的第一个元素
    + 第一项嵌套的第二个元素
    * 第一项嵌套的第三个元素

2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素
* 要有缩进 
总结：（+），（-），（*），（数字点）后面都要加一个空格，否则无效

## MarkDown区块
Markdown 区块引用是在段落开头使用 > 符号 ，然后后面紧跟一个空格符号：

        > 区块引用
        > 菜鸟教程
        > 学的不仅是技术更是梦想
        另外区块是可以嵌套的，一个 > 符号是最外层，两个 > 符号是第一层嵌套，以此类推：
        > 最外层
        > > 第一层嵌套
        > > > 第二层嵌套
        犯得上发生
        大师傅士大夫
        > > 回到第二层

> 区块引用
> 菜鸟教程
> 学的不仅是技术更是梦想
另外区块是可以嵌套的，一个 > 符号是最外层，两个 > 符号是第一层嵌套，以此类推：
> 最外层
> > 第一层嵌套
> > > 第二层嵌套
犯得上发生
大师傅士大夫
> > 回到第二层

## 区块中使用列表

        > + 第一项   
        > * 第二项

> + 第一项
> * 第二项

## 列表中使用区块

    * 第一项
        > 第一项的内容
    * 第二项
        > 第二项的内容

* 第一项
    > 第一项的内容
* 第二项
    > 第二项的内容

## 事项清单
to-do list
\- [x] 已完成项目
    \- [x] 已完成项目1
    \- [x] 已完成项目2
\- [ ] 代办事项
    \- [ ] 代办事项1
    \- [ ] 代办事项2
    \- [ ] 待办事项3

to-do list
- [x] 已完成项目
    - [x] 已完成项目1
    - [x] 已完成项目2
- [ ] 代办事项
    - [ ] 代办事项1
    - [ ] 代办事项2
    - [ ] 待办事项3

## MarkDown代码
如果是段落上的一个函数或片段的代码可以用反引号把它包起来(\`)，例如：
`printf()` 函数 


总结：反引号英文下键盘数字1左边


## 代码区块
* 方法一
代码区块使用 4 个空格或者两个个制表符（Tab 键）。

        class Main{
        public static void main(String args[]){
            System.out.println("Hello MarkDown");
        }
        }

* 方法二
你也可以用 \``` 包裹一段代码，并指定一种语言（也可以不指定）：  

\```java  

class Main{
 public Main(){

 }
}
\```
  
\```c++  

abc  

\```

```java
class Main{
    public Main(){

    }
}
```
```c++
abc
```


总结：方法二结束也要\```,更容易区分代码块

## MarkDown链接
链接使用方法如下：
\[链接名称](链接地址)

或者

\<链接地址>

例子：[百度](http://www.baidu.com)
        or
         <http://www.baidu.com>链接[^footnote]
   [^footnote]: 直接使用链接地址

   总结：脚注\[^变量名] 
   \[^变量名]:
必须以这种格式。

## 高级链接
我们可以通过变量来设置一个链接，变量赋值在文档末尾进行：

        这个链接用 1 作为网址变量 [Google][1]

        [1]: http://www.google.com/

这个链接用 runoob 作为网址变量 [Runoob][runoob]
 [BaiDu][baidu]
然后在文档的结尾为变量赋值（网址）

  
  [runoob]: http://www.runoob.com/
  [baidu]: http://www.baidu.com/

## MarkDown图片
Markdown 图片语法格式如下：

        > \![alt 属性文本](图片地址)
        > \![alt 属性文本](图片地址 "可选标题")

> ![alt 属性文本](图片地址 "鼠标点击显示")
> ![image 美女](./woman.webp "可选标题")


使用实例：

        ![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

        ![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")

        ![image 图标][3]

        [3]: http://static.runoob.com/images/runoob-lgo.png "RUNOOB"
       
	   

[title]: 鼠标悬停显示的文字
        [替换名字]: 当网址失效的时候显示的内容

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")

![image 图标][3]

[3]: http://static.runoob.com/images/runoob-lgo.png "RUNOOB"
[^title]: 鼠标悬停显示的文字
[^替换名字]: 当网址失效的时候显示的内容

        **还无法指定高度宽度**
        <img src="http://static.runoob.com/images/runoob-logo.png" width="50%">

**还无法指定高度宽度**
<img src="./woman.webp" width="50%" height="10%" alt="美女" title="美女">

总结：引用变量只能回车一次之后  
\![图片链接失效显示的文字]\(图片链接 "鼠标悬停显示的内容")

## MarkDwon使用表格
Markdown 制作表格使用 | 来分隔不同的单元格，使用 - 来分隔表头和其他行。

语法格式如下
        |  表头   | 表头  |
        | ---  | ----  |
        | 单元格  | 单元格 |
        | 单元格  | 单元格 |

|  表头   | 表头  |
| ---  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |

## 表格的对齐方式

        | 左对齐 | 右对齐 | 居中 |
        | :----   | ----:   | :---:|
        | 单元格   | 单元格 | 单元格 |

| 左对齐 | 右对齐 | 居中 |
| :---   | ----:   | :---:|
| 单元格   | 单元格 | 单元格 |

| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |

# MarkDown高级技巧
### 支持html标签
不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。

目前支持的 HTML 元素有：\<kbd> \<b> \<i> \<em> \<sup> \<sub> \<br>等 ，如：

        使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑

使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑
### 转义
Markdown 使用了很多特殊符号来表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown 使用反斜杠转义特殊字符：

>  **文本加粗** 
 \*\* 正常显示星号 \*\*

Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号：

> \   反斜线  
\`   反引号  
\*   星号  
\_   下划线  
\{}  花括号  
\[]  方括号  
\()  小括号  
\#   井字号  
\+   加号  
\-   减号  
\.   英文句点  
\!   感叹号  












