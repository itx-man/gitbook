#段落
1.这是一个段落
==><p>这是一个段落。</p>

2.另起一个段落,在两个段落之间隔一个空格。
  这是一个段落。

  这是另一个段落。
==><p>这是一个段落</p>
   <p>这是另一个段落</p>
3.*这是斜体*

4._这也是斜体_

5.**这是粗体**

6.***这是粗体+斜体***

7.~~这是删除线~~

8.markdown总支持1~6六级标题，通过在一行之前加上不同数量的#来表示
#这是H1#
##这是H2##
###这是H3###
...
######这是H6######

这是H1
======
这是H2
------

9.引用，通过在吭首加上大于号>来添加引用格式
>This is a blockquote with two paragraphs.
>>This is nested blockquote. 

10.引用嵌套其他格式
>## 这是一个标题
>
>1.  这是第一行列表项。
>2.  这是第二行列表项。

11.列表
无序列表使用星号、加号或是减号作为列表标记：

*  Red
*  Green
*  Blue

等同于

+  Red
+  Green
+  Blue

和

-  Red
-  Green
-  Blue

有序列表则使用数字接着一个英文句点:

1.  Bird
2.  McHale
3.  Parish

12.内联代码
`System.out.println("Hello World!");`

13.代码区块
```
private Button button;
private Handler handler;
```

14.分隔线
---

15.链接
[an example](http://example.com/)
[an example](http://example.com/"Optional Title")

16.图像
![Alt text](/image.jpg)
![Alt text](/path/to/img.jpg "Optional Title")

17.自动链接
如果链接的地址和名字重复，可以用尖括号语法将其简化。
<http://kancloud.cn/wizardforcel/markdown-simple-world/97375/>
就相当于
[http://example.com/](http://example.com/)

18.转义
markdowm支持在一下字符前面插入反斜杠，插入之后将不再解析这些字符，而是原样输出
```
\   反斜线
`   反引号
*   星号
_   底线
{}  花括号
[]  方括号
()  括弧
#   井字号
+   加号
-   减号
.   英文句点
!   惊叹号
```

19.表格

| Item     | Value | Qty   |
| :------- | ----: | :---: |
| Computer | $1600 |  5    |
| Phone    | $12   |  12   |
| Pipe     | $1    |  234  |

要注意第二行的冒号决定了居左居右还是居中，如果你不加冒号，默认是居左的。

另外可以把第一行去掉，做成没有表头的表格，但第二行始终是要有的。

<table>
<thead>
<tr>
  <th align="left">Item</th>
  <th align="right">Value</th>
  <th align="center">Qty</th>
</tr>
</thead>
<tbody><tr>
  <td align="left">Computer</td>
  <td align="right">$1600</td>
  <td align="center">5</td>
</tr>
<tr>
  <td align="left">Phone</td>
  <td align="right">$12</td>
  <td align="center">12</td>
</tr>
<tr>
  <td align="left">Pipe</td>
  <td align="right">$1</td>
  <td align="center">234</td>
</tr>
</tbody></table>

20. Markdown高级语法
20.1定义列表

 Term 1
 Term 2
 :  Definition A
 :  Definition B

会被编译成

<dl>
<dd>Term 1</dd>
<dd>Term 2</dd>
<dt>Definition A<dt>
<dt>Definition A<dt>
</dl>

22.2 目录

通过[TOC]标记来插入目录

22.3 TeX公式

内联的TeX公式使用一个美元符号标记。

$\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$

会被编译成

TeX公式块用独占一行的两个美元符号来标记。

$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$

会被编译成


22.4 UML图

 '''sequence
 Alice->Bob: Hello Bob, how are you?
 Note right of Bob: Bob thinks
 Bob-->Alice: I am good thanks!
 ```



