#### Latex入门

**资料网址**：

在线LaTeX编辑器：https://www.overleaf.com 

TeX Live下载：https://www.tug.org/texlive/acquire-iso.html 

MikTeX下载：https://miktex.org/download 

LaTeX 公式编辑器：https://latex.codecogs.com/eqneditor/editor.php 

一份不太简短的LaTeX介绍：https://github.com/CTeX-org/lshort-zh-cn

命令以\开头 {}中写参数  []中可选参数

##### 指定文档类型

  文章 article book  report   幻灯片  beamer 

```
\documentclass{article}
```

##### 引用包

```
\usepackage{}
```

##### 文章标题

```
\title{文章的标题}
```

##### 作者名字

```
\author{名字}
```

##### 文档修改日期

```
\date{\today}
```

##### 引言

\maketitle:在当前位置生成文档的标题

##### 文章正文

```
\begin{document}
文章内容
\end{document}
```

##### 常用格式

```
\textbf:加粗文字
\textit:斜体
\underline:下划线
\section{一级章节名}
\subsection{二级章节名}
\subsubsection{三级章节名}
```

##### 插入图片

```
\usepackage{graphicx}

插入位置  添加标题 将图片嵌套进figure环境中
\begin{figure}
\includegraphics[width=0.5\textwidth]{图片名字（可以省略扩展名部分）\textwidth表示当前文本区域的宽度}
\centering:居中显示
\caption{重命名：这是一个网络结构图}
\end{figure}

```

##### 列表

###### 无序列表

```
\begin{itemize}
\item 列表项1
\item 列表项2
\item 列表项3
\end{itemize}
```

###### 有序列表

```
\begin{enumerate}
\item 列表项1
\item 列表项2
\item 列表项3
\end{enumerate}
```

##### 数学公式

可以在任何位置添加公式 被称为 $行内公式$

###### 行间公式

```
\begin{equation}
E=mc^2
\end{equation}
```

###### 复杂公式

```
\begin{equation}
d={k \varphi(n)+1 }\over e
\end{equation}
```

\over 分式  分子在前 分母在后

\varphi 小写

\phi 大写

##### 表格

```
\begin{table}
\center
\begin{tabular}{|l|c|p{2cm}|}
\hline
1&2&3\\
\hline
4&5&6\\
\hline  
7&8&9
\hline\hline
\end{tabular}
\caption{表格名称}
\end{table}
```

{l c c}指定表格格式  l代表左对齐 r代表右对齐 c居中

竖边框|

横边框 \hline

表格内容 每列用&  每行用\\\

\center 居中表格