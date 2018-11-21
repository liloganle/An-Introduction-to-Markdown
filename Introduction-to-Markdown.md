Markdown编辑器及其基础语法介绍
==

<center>作者：Logan </center>

## 1. Moeditor
&emsp;&emsp;本文档是一款名为*Moeditor*的MarkDown语法编辑器编写的，该编辑器已经在Github开源了，它的开源地址在[这里](https://github.com/Moeditor/Moeditor)，它的主页以及下载地址在[这里](https://moeditor.js.org/)。它有如下特点：
- 界面美观、简介
- 支持导出、生成HTML、PDF文档
- 支持Github扩展语法
- 支持TeX数学表达式
- 支出UML图
- 支持编辑时代码高亮
- 含有读、写和预览三种模式
- 可以自定义字体、行高以及字体大小
- 含有多种代码高亮主题
- 支持自动重载
- 支持本地化
- 支持专注模式
- 支持跨平台，涵盖
	- Windows
	- Linux
	- macOS

## 2. Markdown基本语法介绍
### 2.1 标题
&emsp;&emsp;*Markdown*支持两种标题的语法，类`Setext`和类`Atx`形式。类`Setext`是利用底线的形式，并且这种形式只能支持两级标题。在标题底下加上至少两个`=`(在本编辑器是这样的)，用来表示最高阶标题；标题底下加上至少两个`-`，表示第二阶标题。而类`Atx`则是利用在标题前面加上`1~6`个`#`，分别对应一级标题、二级标题，......，六级标题，因此能够支持六级标题。效果如下：

<center>![Setext](https://raw.githubusercontent.com/liloganle/An-Introduction-to-Markdown/master/images/setext.jpg) </center>
<center> 类Setext标题 </center>
<br>
<center>![Atx](https://raw.githubusercontent.com/liloganle/An-Introduction-to-Markdown/master/images/atx.jpg) </center>
<center> 类Atx标题 </center>


### 2.2 段落与换行
&emsp;&emsp;段落之间必须空行，否则两个段落就会合并成为一个段落；同理对于两行文本也是如此，中间不空出一行就会显示成一行文本。如果要在段落内加入换行，则必须使用`<br>`。

&emsp;&emsp;写文章时，我们常常希望`首行缩进`两个汉字字符，这时就需要`&emsp;`。一个`&emsp;`代表缩进一个汉字字符，因此首行缩进两个字符需要用`&emsp;&emsp;`(注意：不要漏掉分号`;`)。

### 2.3 内容引用
&emsp;&emsp;写文章或者的文档的时候，有时需要引用别人的内容，这是就需要引用符号`>`。引用既可以“引用内容”，也可以“多行引用”和“嵌套引用”。引用中也支持标题、列表等其他*Markdown*语法。那么如何在引用中换行呢？在你想要换行的地方至少要键入两个空格之后在按`Enter`或者在引用的内容中加入一个空行就能实现引用内容的换行。但是加入一个空行的效果并没有前一种方法好，两行之间的行距会变宽。为了美观，推荐第一种方法。常见的引用写法及其效果如下图。

<center>![多行引用](https://raw.githubusercontent.com/liloganle/An-Introduction-to-Markdown/master/images/%E5%A4%9A%E8%A1%8C%E5%BC%95%E7%94%A8.png) </center>
<center> 多行引用 </center>
<br>
<center>![嵌套引用](https://raw.githubusercontent.com/liloganle/An-Introduction-to-Markdown/master/images/%E5%B5%8C%E5%A5%97%E5%BC%95%E7%94%A8.png) </center>
<center> 嵌套引用 </center>
<br>
<center>![其他引用](https://raw.githubusercontent.com/liloganle/An-Introduction-to-Markdown/master/images/%E5%85%B6%E4%BB%96%E5%BC%95%E7%94%A8.png) </center>
<center> 其他引用 </center>

### 2.4 列表



代码引用：
```C++
# include<iostream>
int main(void){
	int a,b;
    std::cin >> a >> b;
    std::cout << a + b << std::endl;
    return 0;
}
```



数学公式：
<center>
$ J_{\alpha}(x) = \sum_{m=0}^{\infty} \frac{(-1)^m}{m! \Gamma (m+ \alpha + 1)} (\frac{x}{2})^{2m + \alpha}$
</center>
