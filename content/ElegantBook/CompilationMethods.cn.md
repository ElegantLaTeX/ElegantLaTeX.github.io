---
title: 编译方式
description : "编译方式"
weight: 1
---

本模板基于基础的 book 文类，所以 book 的选项对于本模板也是有效的。默认编码为 UTF-8，推荐使用 TeX Live 编译。本文编写环境为 Win10 (64bit) + TeX Live 2018，支持 `PDFLaTeX` 以及 `XeLaTeX` 编译。

## 选择 PDFLaTeX 编译

如果你使用 `PDFLaTeX` 编译，默认的 Computer Modern 字体被换成了 newtx 系列字体，默认的字体字号是 12 pt。关于字体设置的宏包主要用到了：

+ `newtxtext` 用于文档正文字体，类似于 Times New Roman 字体。
+ `newtxmath` 用于数学字体，搭配 `newtxtext` 非常合适。
+ `FiraMono` 用于打字机字体，并使用了 `scale=0.7` 选项。
+ `ctex` 用于中文字体设置，并使用了 `scheme=plain` 选项。

一次完整的编译：`PDFLaTeX` -> `BibTeX` -> `PDFLaTeX`*2。


## 选择 XeLaTeX 编译

如果你选择 `XeLaTeX` 编译的话，那么设置字体的宏包为 `fontspec` 和 `xeCJK`。由于模板中使用的字体是 Windows 中的字体，所以如果你使用其他操作系统，比如 Linux 或者 Mac OS，那么你需要把所用字体替换为你系统中的字体。设置字体的命令：

```tex
\RequirePackage{fontenc}
\RequirePackage[no-math]{fontspec}
\setmainfont{Times New Roman}[NFSSFamily=ntxtlf]
\setsansfont{Arial}
%\setmonofont[Scale=0.7]{Courier New}
\RequirePackage{xeCJK}
\RequirePackage{xunicode}
\setCJKmainfont[BoldFont={SimHei},ItalicFont={KaiTi}]{SimSun}
\setCJKsansfont[BoldFont={SimHei},ItalicFont={KaiTi}]{KaiTi}
\setCJKmonofont[BoldFont={SimHei},ItalicFont={KaiTi},Scale=0.7]{Microsoft YaHei}
\XeTeXlinebreaklocale ”zh”
\XeTeXlinebreakskip = 0pt plus 1pt minus 0.1pt
\RequirePackage{newtxmath}
```

一次完整的编译：`XeLaTeX` -> `BibTeX` -> `XeLaTeX`*2。
