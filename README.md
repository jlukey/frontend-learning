> **笔记来源**：尚硅谷前端html+css零基础教程，2023最新前端开发html5+css3视频(禹神)
<!--ts-->
* [一、前序知识](#一前序知识)
   * [1. 认识两位先驱](#1-认识两位先驱)
   * [2. 计算机基础知识](#2-计算机基础知识)
   * [3. C/S架构与B/S架构](#3-cs架构与bs架构)
   * [4. 浏览器相关知识](#4-浏览器相关知识)
   * [5. 网页相关概念](#5-网页相关概念)
* [二、HTML 简介](#二html-简介)
  
   * [1. 什么是 HTML](#1-什么是-html)
   * [2. 相关国际组织](#2-相关国际组织)
   * [3. HTML发展史](#3-html-发展历史)
* [三、HTML 入门](#三html-入门)
   
   * [1. HTML 初体验](#1-html-初体验)
   * [2. HTML 标签](#2-html-标签)
   * [3. HTML 标签属性](#3-html-标签属性)
   * [4. HTML 基本结构](#4-html-基本结构)
   * [5. 安装 VSCode](#5-安装-vscode)
   * [6. 安装 Live Server 插件](#6-安装-live-server-插件)
   * [7. HTML 注释](#7-html-注释)
   * [8. HTML 文档声明](#8-html-文档声明)
   * [9. HTML 字符编码](#9-html-字符编码)
   * [10. HTML 设置语言](#10-html-设置语言)
   * [11. HTML标准结构](#11-html标准结构)
* [四、HTML 基础](#四html-基础)
   * [1. 开发者文档](#1-开发者文档)
   * [2. 排版标签](#2-排版标签)
   * [3. 语义化标签](#3-语义化标签)
   * [4. 块级元素 与 行内元素](#4-块级元素-与-行内元素)
   * [5 .文本标签_常用的](#5-文本标签_常用的)
      * [6 .文本标签_不常用的](#6-文本标签_不常用的)

<!--te-->

# 一、前序知识

## 1. 认识两位先驱
![](https://i-blog.csdnimg.cn/blog_migrate/7f2de089c547b15fe3c77538769a27e9.png)

## 2. 计算机基础知识
**计算机** 俗称电脑，是现代一种用于高速计算的电子计算机器，可以进行数值计算、逻辑计算，还具有存储记忆功能。

计算机由 **硬件** + **软件** 组成。

**计算机硬件**是指计算机系统中的物理组件和设备，包括处理器（CPU）、内存、硬盘、显示器、键盘、鼠标等。硬件是实际存在的物理实体，它们通过电子信号、电流等方式来执行计算和处理任务。硬件提供了计算机系统的基本功能和执行计算任务的能力。

**计算机软件**是指安装在计算机系统中的程序和数据。软件是一系列指令的集合，可以告诉计算机硬件如何执行特定的任务。软件包括操作系统、应用程序、驱动程序等。软件在计算机系统中是以二进制代码的形式存在，可以被计 算机硬件识别和执行。



**软件的分类**：

系统软件：Windows、Linux、Android、Harmony 等。

应用软件：微信、QQ、王者荣耀、PhotoShop 等。

整体图示：
![](https://i-blog.csdnimg.cn/blog_migrate/d33fe0138c975f1c065613ce8a3ca19b.jpeg)

## 3. C/S架构与B/S架构

上面提到的应用软件，又分为两大类：
* C/S架构 ，特点：需要安装、偶尔更新、不跨平台、开发更具针对性。
* B/S架构 ，特点：无需安装、无需更新、可跨平台、开发更具通用性。
>  名词解释：C => client（客户端）、B => browser（浏览器）、S => server（服务器）

前端工程师主要负责编写 B/S架构中的网页（呈现界面、实现交互）。

> ​        大前端时代指的是当前互联网技术发展的趋势，前端开发的范围和重要性不断扩大，成为了互联网行业中一个重要的领域。在大前端时代，前端开发不再局限于传统的网页展示和交互，而是涉及到更广泛的领域和技术，包括移动应用、桌面应用、跨平台开发、物联网应用等。



## 4. 浏览器相关知识

浏览器是网页运行的平台，常见的浏览器有：谷歌(Chrome)、Safari、IE 、火狐(Firefox)、欧
朋(Opera)等，以上这些是常用的五大浏览器。



**各大浏览器市场份额:**

![](https://i-blog.csdnimg.cn/blog_migrate/48796ad7795493b4e67c457911f9e67d.jpeg)



**这里简单提及为什么前端开发多使用chrome浏览器 ?**

1. **谷歌Chrome浏览器界面简洁**，清爽干净，性能也是非常好的。
2. **速度快**。相比于猎豹、IE等浏览器，谷歌Chrome浏览器的加载速度可谓第一。由于采用多进程架构，一个站点的加载速度较慢不会拖累对其它站点的访问。
3. **插件资源丰富**。谷歌Chrome浏览器拥有强大的第三方插件库，因此使用起来极其方便。
4. **支持HTML5全面以及浏览器兼容问题**。前端程序员那么喜欢chrome，就是因为兼容起来最简单！而且HTML5和CSS3可以给用户带来高一层次的视觉和体验。
5. **系统不会崩溃**。Chrome的亮点就是其多进程架构，保护浏览器不会因恶意网页和应用软件而崩溃。
6. **开发者工具**。最开始的时候，chrome开发者工具跟IE差不多，也不怎么不好用，不过一次一次的迭代，现在的chrome开发者工具已经超过firebug了。



**常见浏览器的内核 :**

浏览器的内核是指浏览器所使用的渲染引擎，它负责解析和渲染网页内容，将 HTML、CSS 和 JavaScript 代码转换成可视化的网页。不同浏览器使用不同的内核，每个内核都有其独特的实现方式和特点。

![](https://i-blog.csdnimg.cn/blog_migrate/e7d90238df7b070bd569972258aad59b.jpeg)



1. 解析HTML和CSS：内核负责解析HTML和CSS代码，并将其转换成可视化的网页。
2. 处理网页布局：内核根据HTML和CSS规则来确定网页的布局方式，包括元素的定位、大小、层叠等。
3. 执行JavaScript代码：内核执行网页中的JavaScript代码，处理交互逻辑、动态效果等。
4. 渲染网页内容：内核将解析后的网页内容渲染到屏幕上，包括文字、图像、多媒体等元素的显示。
5. 处理用户交互：内核响应用户的操作，处理点击、滚动、表单提交等交互行为。



## 5. 网页相关概念

**网址**：我们在浏览器中输入的地址。

**网页**：浏览器所呈现的每一个页面。

**网站**：多个网页构成了一个网站。

**网页标准**：网页标准是由国际标准组织和技术组织制定的一系列规范和指南，用于确保网页在不同浏览器中具有一致的展现效果，并推动Web技术的发展。

以下是一些常见的网页标准：

* HTML（Hypertext Markup Language）：HTML定义了网页的结构和内容标记，包括标题、段落、链接、图像等元素，目前最新的版本是HTML5。

* CSS（Cascading Style Sheets）：CSS用于描述网页的样式和布局，通过选择器和属性来设置网页元素的外观和排版。

* JavaScript：JavaScript是一种脚本语言，用于为网页添加交互行为和动态效果，可以操作网页的内容、样式和行为。

![](https://i-blog.csdnimg.cn/blog_migrate/fbdb2324a66840b438633477267ac193.jpeg)



# 二、HTML 简介

## 1. 什么是 HTML

HTML全称：**HyperText Markup Language（超文本标记语言）。**

> **超文本**：暂且简单理解为 "超级的文本"，和普通文本比，内容更丰富。
>
> **标 记**：文本要变成超文本，就需要用到各种标记符号。
>
> **语 言**：每一个标记的写法、读音、使用规则，组成了一个标记语言。

## 2. 相关国际组织

**IETF**:

全称：Internet Engineering Task Force（国际互联网工程任务组），成立于 1985 年底，是一个权威的互联网技术标准化组织，主要负责互联网相关技术规范的研发和制定，当前绝大多数国际互联网技术标准均出自IETF。

官网： https://www.ietf.org



**W3C**:

全称：World Wide Web Consortium（万维网联盟），创建于 1994 年，是目前Web技术领域，最具影响力的技术标准机构。共计发布了 200 多项技术标准和实施指南，对互联网技术的发展和应用起到了基础性和根本性的支撑作用，

官网： https://www.w3.org



**WHATWF**:

全称：Web Hypertext Application Technology Working Group（网页超文本应用技术工作小组）成立于 2004 年，是一个以推动网络HTML 5 标准为目的而成立的组织。由Opera、Mozilla基金会、苹果，等这些浏览器厂商组成。

官网： https://whatwg.org/



## 3. HTML发展史

从 HTML 1. 0 开始发展，期间经历了很多版本，目前HTML的最新标准是：HMTL 5 ，具体发展史如图.

![](https://i-blog.csdnimg.cn/blog_migrate/71d3d089f0ac36aa8613e98ae04a714e.jpeg)



# 三、HTML 入门

## 1. HTML 初体验

1. 第一步：鼠标右键 => 新建 => 文本文档 => 输入以下内容，并保存。

   ```html
   <marquee>这里就随便你输什么啦,会滚动的哟</marquee>
   ```

2. 第二步：修改后缀为.html，然后双击打开即可。（这里的后缀名，使用.htm也可以，但推荐使用更标准的.html）

3. 程序员写的叫**源代码** ，要交给浏览器进行渲染。

4. 借助浏览器看网页的源代码 ，具体操作：在网页空白处鼠标右键 ==> 查看网页源代码。

## 2. HTML 标签

1. 标签 又称 元素 ，是HTML的基本组成单位。

2. 标签分为： 双标签 与 单标签 （绝大多数都是双标签）。

3. 标签名不区分大小写，但推荐小写，因为小写更规范。

4. 双标签：

   ![](https://i-blog.csdnimg.cn/blog_migrate/f8fea3d20623962a25fff293cddf94da.jpeg)

   

5. 单标签

   ![](https://i-blog.csdnimg.cn/blog_migrate/2ea09de5f5caf8656431af1aefbc4152.jpeg)

6. 标签之间的关系：并列关系、嵌套关系，可以使用tab键进行缩进。

   ```html
   <marquee loop="1" bgcolor="orange" id="asdfasd">
   	hello world!
   	<input type="password"> 	
   </marquee>
   <input>
   <input disabled>
   ```

## 3. HTML 标签属性

**作用**：用于给标签提供 附加信息

**使用方式**：可以写在**起始标签**或**单标签**中 ，形式如下：

![](https://i-blog.csdnimg.cn/blog_migrate/6552d3882c7013ed360f2a6b7ad593e5.jpeg)

```html
<marquee loop = "1" bgcolor="orange">图南</marquee>
<input type="password">
```

> 有些特殊的属性，没有属性名，只有属性值，例如: <input disabled>



**注意点**：

1. 不同的标签，有不同的属性；也有一些通用属性（在任何标签内都能写，后面会详细总结）。
2. 属性名、属性值不能乱写，都是W 3 C规定好的。
3. 属性名、属性值，都不区分大小写，但推荐小写。
4. 双引号，也可以写成单引号，甚至不写都行，但还是推荐写双引号。
5. 标签中不要出现同名属性，否则后写的会失效，例如：

```html
<input type="text" type="password">
```



## 4. HTML 基本结构

1. 在网页中，如何查看某段结构的具体代码？—— 点击鼠标右键，选择“检查”。

2. **检查** 和 **查看网页源代码** 的区别：

   - 【查看网页源代码】看到的是：程序员编写的源代码。
   - 【检查】看到的是：经过浏览器 “处理” 后的源代码。
   -   备注：日常开发中，【检查】用的最多。

3. 网页的 **基本结构** 如下：

   1. 想要呈现在网页中的内容写在body标签中。 
   2. head标签中的内容不会出现在网页中。 
   3. head标签中的title标签可以指定网页的标题。

4. 图示：![](https://i-blog.csdnimg.cn/blog_migrate/9e6f666b64cab3f435c1c90292ed4d45.jpeg)

5. 代码示例：

   ```html
   <html>
       <head>
           <title>网页标题</title>
       </head>
       <body>
           ......
       </body>
   <html>
   ```



## 5. 安装 VSCode

1. 安装中文语言包。
2.  使用 VSCode打开文件夹的两种方式。 
3. 调整字体大小。
4.  设置主题。 
5. 安装图标主题：vscode-icons。



## 6. 安装 Live Server 插件

1. 可以更加方便的打开网页。
2. 打开网页的方式更贴近项目上线。
3. 代码出现改动后，可以自动刷新。
4. 根据自己的情况，去配置一下 VSCode 的自动保存。

> **注意事项** ：
>
> * 务必使用VSCode打开的是文件夹，否则 Live Server 插件无法正常工作！
> * 打开的网页必须是标准的HTML结构，否则无法自动刷新！



## 7. HTML 注释

1. 特点：注释的内容会被浏览器所忽略，不会呈现到页面中，但源代码中依然可见。

2. 作用：对代码进行解释和说明。

3. 写法：

   ```html
   <!-- 下面的文字只能滚动一次 -->
   <marquee loop="1">火影忍者</marquee>
   ```

   ```html
   <!-- 下面的文字可以无限滚动 -->
   <marquee>犬夜叉</marquee>
   ```

   

4. 注释不可以嵌套，以下这么写是错的（反例）。

   ```html
   <!--
   	我是一段注释
   	<!-- 我也是一段注释 -->
   -->
   ```



## 8. HTML 文档声明

作用：告诉浏览器当前网页的版本。

写法：`<!DOCTYPE html>` 或 `<!DOCTYPE HTML>` 或 `<!doctype html>`

>  注意：文档声明，必须在网页的第一行，且在**html标签的外侧**。



## 9. HTML 字符编码

**计算机对数据的操作**：

- 存储时，对数据进行：编码。
- 读取时，对数据进行：解码。

**编码、解码，会遵循一定的规范 —— 字符集**。

**字符集有很多中，常见的有以下几种**（了解）：

```markdown
ASCII：大写字母、小写字母、数字、一些符号，共计 128 个。
ISO8859-1：在 ASCII 基础上，扩充了一些希腊字符等，共计是 256 个。
GB2312：继续扩充，收录了 6763 个常用汉字、 682 个字符。
GBK：收录了的汉字和符号达到 20000 + ，支持繁体中文。
UTF-8：包含世界上所有语言的：所有文字与符号。—— 很常用。
```

**使用原则是怎样的？**

* 原则1：存储时，务必采用合适的字符编码 。否则会导致无法存储，数据会丢失！

* 原则2：存储时采用哪种方式编码 ，读取时就采用哪种方式解码。否则会导致数据错乱（乱码）！



例如下面文字中，包含有：中文、英文、泰文、缅甸文。

```
我爱你
I love you!
ฉันรักเธอนะ
ကန်မကိ ချစ်တယ်။
```

> 若使用 ISO8859- 1 编码存储，在存入的那一刻，就出问题了，因为ISO8859- 1 仅支持英文！
>
> 为保证所有的输入，都能正常存储和读取，现在几乎全都采用：UFT- 8 编码。
>
> 所以我们编写html文件时，也都统一用UFT- 8 编码。

总结：

- 平时编写代码时，统一采用UTF- 8 编码（最稳妥）。
- 为了让浏览器在渲染html文件时，不犯错误，可以通过meta标签配合charset属性指定字符编码。

```html
<head>    
  	<meta charset="UTF-8"/> 
</head>
```



## 10. HTML 设置语言

**主要作用：**

- 让浏览器显示对应的翻译提示。
- 有利于搜索引擎优化。

**具体写法：**

```html
<html lang="zh-CN">
```

> 扩展知识：lang属性的编写规则（作为一个课外扩展知识，了解即可）。
>
> 1. 第一种写法（ 语言-国家/地区 ），例如：
>
>    * zh-CN ：中文-中国大陆（简体中文）
>    * zh-TW ：中文-中国台湾（繁体中文）
>    * zh ：中文
>    * en-US ：英语-美国
>    * en-GB ：英语-英国
>
> 2. 第二种写法（ 语言—具体种类）已不推荐使用，例如：
>
>    * zh-Hans ：中文—简体
>    * zh-Hant ：中文—繁体
>
> 3. W3School 上的说明： [《语言代码参考手册》](https://www.w3school.com.cn/tags/html_ref_language_codes.asp) 、 [《国家/地区代码参考手册》](https://www.w3school.com.cn/tags/html_ref_country_codes.asp)
>
> 4. W3C官网上的说明： [《Language tags in HTML》](https://www.w3.org/International/articles/language-tags/)
>
>    ![](https://i-blog.csdnimg.cn/blog_migrate/14b0b494621083e4de2bb67115c11143.jpeg)

## 11. HTML标准结构

HTML标准结构如下：

输入!，随后回车即可快速生成标准结构。

生成的结构中，有两个meta标签，我们暂时用不到，可以先删掉。
配置VScode的内置插件emmet，可以对生成结构的属性进行定制。
在存放代码的文件夹中，存放一个favicon.ico图片，可配置网站图标。



# 四、HTML 基础

## 1. 开发者文档

- **W3C官网**：www.w3c.org
- **W3School**：www.w3school.com.cn
- **MDN**：developer.mozilla.org —— 平时用的最多(貌似更新了AI模式，有空可以去了解一下)。

## 2. 排版标签

| 标签名 | 标签含义                                     | 单/双标签 |
| ------ | -------------------------------------------- | --------- |
| h1~h6  | 标题                                         | 双        |
| p      | 段落                                         | 双        |
| div    | 没有任何含义，用于整体布局（生活中的包装袋） | 双        |

1. h1最好写一个，h2~h6能适当多写。
2. h1~h6不能互相嵌套，例如：h1 标签中最好不要写h2 标签了。
3. p 标签很特殊！它里面不能有：**h1~h6、p、div标签**（暂时先这样记，后面会说规律）。

## 3. 语义化标签

**概念：**用特定的标签，去表达特定的含义。

**原则：**标签的默认效果不重要（后期可以通过CSS随便控制效果），语义最重要！

**举例：**对于h1标签，效果是文字很大（不重要），语义是网页主要内容（很重要）。

**优势：**

- 代码结构清晰可读性强。
- 有利于 **SEO** （搜索引擎优化）。(爬虫 代码 机器人)
- 方便设备解析（如屏幕阅读器、盲人阅读器等）。



## 4. 块级元素 与 行内元素
**块级元素** ：独占一行（排版标签都是块级元素）。
**行内元素** ：不独占一行（目前只学了：input，稍后会学习更多）。
**使用原则** ：

* 块级元素 中能写 行内元素 和 块级元素 （简单记：块级元素中几乎什么都能写）。

* 行内元素 中能写 行内元素 ，但不能写 块级元素 。

* 一些特殊的规则：h1~h6 不能互相嵌套、 p标签中不要写块级元素。

>  marquee元素设计的初衷是：让文字有动画效果，但如今我们可以通过CSS来实现了，而且还可以实现的更加炫酷，所以marquee标签已经： 过时了 （废弃了），不推荐使用。我们只是在开篇的时候，用他做了一个引子而已，在后续的学习过程中，这些已经废弃的标签，我们直接跳过。



## 5 .文本标签_常用的

1. 用于包裹：词汇、短语等。
2. 通常写在排版标签里面。
3. 排版标签更宏观（大段的文字），文本标签更微观（词汇、短语）。

| 标签名 | 标签语义                         | 单/双标签 |
| ------ | -------------------------------- | --------- |
| em     | 要着重阅读的内容                 | 双        |
| strong | 十分重要的内容（语气比 em 要强） | 双        |
| span   | 没有语义，用于包裹短语的通用容器 | 双        |

> 生活中的例子**：div是大包装袋，span是小包装袋。**

## 6 .文本标签_不常用的

| 标签名 | 标签语义                                           | 单/双标签 |
| ------ | -------------------------------------------------- | --------- |
| cite   | 作品标题（书籍、歌曲、电影、电视节目、绘画、雕塑） | 双        |
| dfn    | 特殊术语，或专属名词                               | 双        |
| del    | 删除的文本【与】插入的文本                         | 双        |
| ins    | 插入的文本【与】删除的文本                         | 双        |
| sub    | 下标文字【与】上标文字                             | 双        |
| sup    | 上标文字【与】下标文字                             | 双        |
| code   | 一段代码                                           | 双        |
|        |                                                    |           |

| samp | 从正常的上下文中，将某些内容提取出来 | 双   |
| ---- | ------------------------------------ | ---- |
| kbd  | 键盘文本，表示文本是通过键盘输入的   | 双   |

|       |                                    |      |
| ----- | ---------------------------------- | ---- |
| abbr  | 缩写，最好配合上 title 属性        | 双   |
| bdo   | 更改文本方向，要配合 dir 属性      | 双   |
| var   | 标记变量，可以与 code 标签一起使用 | 双   |
| small | 附属细则，例如：包括版权、法律文本 |      |

| b          | 摘要中的关键字、评论中的产品名称                     | 双   |
| ---------- | ---------------------------------------------------- | ---- |
| i          | 人物的思想活动、所说的话等                           | 双   |
| u          | 与正常内容有反差文本，例如：错的单词、不合适的描述等 | 双   |
| q          | 短引用                                               | 双   |
| blockquote | 长引用                                               | 双   |
| address    | 地址信息                                             | 双   |
