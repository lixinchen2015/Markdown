# Markdown语法

> [Markdown 官方教程](https://markdown.com.cn/cheat-sheet.html)

## 一、纯文本基本语法
### 1.标题

在行首插入 1 到 6 个 # ，对应到标题 1 到 6 阶，示例：

```# this is H1```  
```## this is H2```  
```###### this is H6```

### 2.字体
使用星号（ * ）和底线（ _ ）作为标记强调字词的符号，你可以随便用你喜欢的样式，唯一的限制是，你用什么符号开启标签，就要用什么符号结束。写中文时还是（ * ）比较好用，因为它不区分全角半角，不用切换输入法。 示例：

**```**这是加粗**```**  
__```__这也是加粗__```__  
*```*这是倾斜*```*  
_```_这也是倾斜_```_  
***```***这是加粗倾斜***```***  
~~```~~这是加删除线~~```~~  

### 3.分割线
你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。

你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：

```* * *```  
```***```  
```**********```  
```- - -```  
```_________________```
    
ps:为了兼容性，请在分隔线的前后均添加空白行。

### 4.引用
在引用的文字前加 > 即可。 在 Markdown 文件中建立一个区块引用，那会看起来像是你自己先断好行，然后在每行的最前面加上 > ：

```> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,```  
```> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.```  
```> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.```  
```> ```  
```> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse```  
```> id sem consectetuer libero luctus adipiscing.```

效果如下：
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

Markdown 也允许你偷懒只在整个段落的第一行最前面加上 > ：

```> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,```  
```  consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.```  
```  Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.```  
```> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse```  
```  id sem consectetuer libero luctus adipiscing.```

区块引用可以嵌套（例如：引用内的引用），只要根据层次加上不同数量的 > ：

```> This is the first level of quoting.```  
```> > This is nested blockquote.```  
```> > > > Back to the first level.```

效果如下：
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> > > > Back to the first level.

引用的区块内也可以使用其他的 Markdown 语法，包括标题、列表、代码区块等：
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.

### 5.列表
#### 有序列表
有序列表则使用数字接着一个英文句点作为标记。 示例：

```1. 列表内容```  
```2. 列表内容```  
```3. 列表内容```

1. 列表内容
2. 列表内容
3. 列表内容

ps:序号跟内容之间要有空格

#### 无序列表
创建无序列表，请在每个列表项前面添加破折号 ( - )。缩进一个或多个列表项可创建嵌套列表。示例：

```- First item```  
```- Second item```  
```- Third item```  
```- Fourth item```

- First item
- Second item
- Third item
- Fourth item

要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符。示例：

*   This is the first list item.  
    I need to add another paragraph below the second list item.
*   Here's the second list item.
    > A blockquote would look great below the second list item.
*   And here's the third list item.

代码块通常采用四个空格或一个制表符缩进。当它们被放在列表中时，请将它们缩进八个空格或两个制表符。示例：

1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.

### 6.代码块

要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符。

    select * from EXP_ASSET_EXT_BILL_DL;

### 7.超链接

链接文本放在中括号内，链接地址放在后面的括号中。链接title是当鼠标悬停在链接上时会出现的文字，这个title是可选的，它放在圆括号中链接地址后面，跟链接地址之间以空格分隔。

超链接Markdown语法代码：```[超链接显示名](超链接地址 "超链接title")。```示例：

Markdown语法请参考 [Markdown语法](https://markdown.com.cn "最好的markdown教程")。

引用类型链接：

[hobbit-hole][1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle

ps:URL中间的空格方式不一样。为了兼容性，请尽量使用%20代替空格。如：( https://www.example.com/my%20great%20page )

### 8.图片
插入图片Markdown语法代码：

```![图片alt](图片链接 "图片title")。```  
示例：
```![这是图片](./assets/img/无尽的楼梯通向天堂，天空充满了云.jpg "无尽的楼梯通向天堂，天空充满了云")```

![这是图片](./assets/img/无尽的楼梯通向天堂，天空充满了云.jpg "无尽的楼梯通向天堂，天空充满了云")

给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。  
示例：
```[![绿洲的岩石图片](./assets/img/绿洲的岩石.jpg "绿洲的岩石")](https://github.com/lixinchen2015/Markdown-/blob/main/Readme.md)```

[![绿洲的岩石图片](./assets/img/绿洲的岩石.jpg "绿洲的岩石")](https://github.com/lixinchen2015/Markdown-/blob/main/Readme.md)

### 9.转义字符
要显示原本用于格式化 Markdown 文档的字符，请在字符前面添加反斜杠字符 \ 。

```\* Without the backslash, this would be a bullet in an unordered list. ```  
\* Without the backslash, this would be a bullet in an unordered list.

在文件中插入一个著作权的符号，你可以这样写：
```&copy```:&copy;

---

## 二、扩展语法
### 1.Markdown 表格

要添加表，请使用三个或多个连字符（---）创建每列的标题，并使用管道（|）分隔每列。您可以选择在表的任一端添加管道。

```| Syntax    | Description |```  
```| ---------- | ----------- |```  
```| Header    | Title     |```  
```| Paragraph  | Text      |```

| Syntax     | Description |
| -----------  | ----------- |
| Header     | Title     |
| Paragraph   | Text      |

ps:使用[Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)可通过图形界面构建表，然后将生成的Markdown格式的文本复制到文件中。

### 2.围栏代码块
Markdown基本语法允许您通过将行缩进四个空格或一个制表符来创建代码块。如果发现不方便，请尝试使用受保护的代码块。根据Markdown处理器或编辑器的不同，您将在代码块之前和之后的行上使用三个反引号（ ``` ）。要添加语法突出显示，请在受防护的代码块之前的反引号旁边指定一种语言。

    ```SQL
    {
      select * from EXP_ASSET_EXT_BILL_DL;
    }
    ```  
呈现的输出如下所示：
```SQL
{
  select * from EXP_ASSET_EXT_BILL_DL;
}
```

### 3.脚注
脚注使您可以添加注释和参考，而不会使文档正文混乱。当您创建脚注时，带有脚注的上标数字会出现在您添加脚注参考的位置。读者可以单击链接以跳至页面底部的脚注内容。

要创建脚注参考，请在方括号```[^1]```内添加插入符号和标识符。标识符可以是数字或单词，但不能包含空格或制表符。标识符仅将脚注参考与脚注本身相关联-在输出中，脚注按顺序编号。

在括号内使用另一个插入符号和数字添加脚注，并用冒号和文本```[^1]: 我的脚注```。您不必在文档末尾添加脚注。您可以将它们放在除列表，块引号和表之类的其他元素之外的任何位置。

这是第一个脚注，[^1] 这是一个长脚注。[^bignote]

[^1]:   这是第一个脚注。

[^bignote]: 这是一个有多个段落和代码的例子。  
            缩进段落以将其包含在脚注中。  
            可在脚注中插入代码：`｛我的代码｝`  
            脚注可添加任意多的段落。
    
### 4.任务列表
要创建任务列表，请在任务列表项之前添加破折号-和方括号[ ]，并在[ ]前面加上空格。要选择一个复选框，请在方括号[x]之间添加 x 。

```- [x] Write the press release```  
```- [ ] Update the website```  
```- [ ] Contact the media```

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

---

## 三、公式
[数学公式汇总（Markdown）](https://zhuanlan.zhihu.com/p/261750408)

### 1.公式块
```在文中输入($$)，再按下回车：```  
```$$```  
```h_\theta(x)=\theta_0+\theta_1*x```  
```$$```

$$
h_\theta(x)=\theta_0+\theta_1*x
$$

### 2.行内公式
在文中输入```($_$)```，将公式嵌入文字内：  
```自变量$\theta$增大，函数$\theta^2$随之增大。```  
自变量$\theta$增大，函数$\theta^2$随之增大。
### 3.常用符号
|  符  号  | 数学表达式 | Latex代码 |
| ---------- | ---------- | --------- |
| 上  标 | $x^2$      | ```x^2``` |
| 下  标 | $y_1$ | ```y_1``` |
| 正无穷 | $+\infty$ | ```+\infty``` |
| 负无穷 | $-\infty$ | ```-\infty``` |
| 加减乘 | $a\*b-c$ | ```a*b-c``` |
|  除  | $a\div{b}$ | ```a\div{b}``` |
|  分式  | $\frac{a}{b}$ | ```\frac{a}{b}``` |
| 正负号 | $a\pm{d}$ | ```a\pm{d}``` |
| 根  号 | $\sqrt{x}$ | ```\sqrt{x}``` |
| 省略号 | $\cdots$ | ```\cdots``` |
| 三角函数 | $\sin{\theta}$ | ```\sin{\theta}``` |
| 向量 | $\vec{a}$ | ```\vec{a}``` |
| 向量 | $\overleftarrow{AB}$ | ```\overleftarrow{AB}``` |
| 向量 | $\overrightarrow{AB}$ | ```\overrightarrow{AB}``` |
| 累加 | $\sum_{i=1}^{n}{a_i}$ | ```$\sum_{i=1}^{n}{a_i}$``` |
| 累乘 | $\prod_{i=1}^{n}{a_i}$ | ```$\prod_{i=1}^{n}{a_i}$``` |


### 4.公式序号
公式最后的一行即表示右端序号。示例：  
```$$```  
```h_\theta(x)=\theta_0+\theta_1*x```  
```\tag{1}```  
```$$```

$$
h_\theta(x)=\theta_0+\theta_1*x
\tag{1}
$$
### 5.矩阵
#### 1.简单矩阵
使用```\begin{matrix}…\end{matrix}```生成， 每一行以```\\```结尾表示换行，元素间以```&```间隔，式子的表示序号```\tag{1}```（右边的序号）。
```
$$
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\tag{2}
$$
```

$$
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\tag{2}
$$

#### 2.带左右括号的矩阵(大中小括号)
在```\begin{}```之前和```\end{}之后```添加左右括号的代码。
- 大括号
```
$$
\left\\{  
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right\\}
\tag{3}
$$
```

$$
\left\\{  
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right\\}  
\tag{3}
$$

- 中括号
```
$$
\left\[
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right\]
\tag{4}
$$
```
$$
\left\[
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right\]
\tag{4}
$$

- 小括号

```
$$
\left\(
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right\)
\tag{5}
$$
```
$$
\left\(
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right\)
\tag{5}
$$

#### 3.包含希腊字母与省略号
行省略号\cdots，列省略号\vdots，斜向省略号（左上至右下）\ddots。
```
$$
 \left\\{
 \begin{matrix}
 1      & 2        & \cdots & 5        \\
 6      & 7        & \cdots & 10       \\
 \vdots & \vdots   & \ddots & \vdots   \\
 \alpha & \alpha+1 & \cdots & \alpha+4 
 \end{matrix}
 \right\\}
$$
```
$$
 \left\\{
 \begin{matrix}
 1      & 2        & \cdots & 5        \\
 6      & 7        & \cdots & 10       \\
 \vdots & \vdots   & \ddots & \vdots   \\
 \alpha & \alpha+1 & \cdots & \alpha+4 
 \end{matrix}
 \right\\}
$$
### 6.行列式
```
$$
 \begin{vmatrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{vmatrix}
\tag{6}
$$
```
$$
 \begin{vmatrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{vmatrix}
\tag{6}
$$
### 7.真值表
```
$$
\begin{array}{cc|c}
A&B&F\\
\hline
0&0&0\\
0&1&1\\
1&0&1\\
1&1&1\\
\end{array}
$$
```
$$
\begin{array}{cc|c}
A&B&F\\
\hline
0&0&0\\
0&1&1\\
1&0&1\\
1&1&1\\
\end{array}
$$
### 8.多行等式对齐
```
$$
\begin{aligned}
a &= b + c \\
  &= d + e + f
\end{aligned}
$$
```
$$
\begin{aligned}
a &= b + c \\
  &= d + e + f
\end{aligned}
$$
### 9.方程组、条件表达式
- 方程组
```
$$
\begin{cases}
3x + 5y +  z \\
7x - 2y + 4z \\
-6x + 3y + 2z
\end{cases}
\tag{7}
$$
```
$$
\begin{cases}
3x + 5y +  z \\
7x - 2y + 4z \\
-6x + 3y + 2z
\end{cases}
\tag{7}
$$
- 条件表达式
```
$$
f(n) =
\begin{cases} 
n/2,  & \text{if }n\text{ is even} \\
3n+1, & \text{if }n\text{ is odd}
\end{cases}
\tag{8}
$$
```
$$
f(n) =
\begin{cases} 
n/2,  & \text{if }n\text{ is even} \\
3n+1, & \text{if }n\text{ is odd}
\end{cases}
\tag{8}
$$

### 10.间隔 (大小空格、紧贴)
紧贴 + 无空格 + 小空格 + 中空格 + 大空格 + 真空格 + 双真空格
```
$$
a\!b + ab + a\,b + a\;b + a\ b + a\quad b + a\qquad b
$$
```
$$
a\!b + ab + a\,b + a\;b + a\ b + a\quad b + a\qquad b
$$

### 11.在线编写生成Latex表达式

[Latex公式](https://latexlive.com/)

### 12.通过Python生成Latex表达式
```python
{
    import math//引入数学模块(有些运算的函数需要)  
    import latexify//引入latexify模块  
    
    @latexify.with_latex//特定语法，表示之后定义的函数可以转化为LaTeX代码  
    def f(x,y,z)://包含的参数  
        pass   //此处填写可能需要的数学表达式  
        return result//也可以直接体现数学关系  
    
    print(f)   //直接print(函数名)
}
```


