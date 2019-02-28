---
title: ElegantBook
weight: 2
pre: "<b>2. </b>"
---

值此版本发行之际，我们 ElegantLaTeX 项目组向大家重新介绍一下我们的工作，我们致力于打造一系列美观、优雅、简便的模板方便用户使用。ElegantLaTeX 系列模板目前由 [ElegantNote](https://github.com/ElegantLaTeX/ElegantNote)，[ElegantBook](https://github.com/ElegantLaTeX/ElegantBook)，[ElegantPaper](https://github.com/ElegantLaTeX/ElegantPaper) 组成，分别用于排版笔记，书籍和工作论文。这些子项目的名词是一体的，请在使用这些名词的时候不要将其断开（如 Elegant Note 是不正确的写法）。并且，ElegantLaTeX Book 指的即是 ElegantBook。

最新版本下载地址：[Github:ElegantBook/releases](https://github.com/ElegantLaTeX/ElegantBook/releases)。本文将介绍本模板的一些设置内容以及基本使用方法。如果您有其他问题，建议或者意见，欢迎联系我们。

## ElegantBook 更新说明

在这几年间，我们收到了很多用户的反馈，主要的问题涉及到字体安装，编码支持，定理浮动，定理跨页，交叉引用等等。我们思前想后，原先让用户安装字体以追求视觉上的美观并不完美，用户陷入了巨大的麻烦，这违背了我们的模板初衷。因此我们在新版中删除了这部分，用户无需安装任何字体。让我们来看下此次 ElegantBook 模板 3.x 更新的主要内容有：

1. 删除了自定义字体设置，改用 `ctex` 宏包或者系统默认字体；
2. 模板拆分为中英文模式（`lang=cn/en`）；
3. `PDFLaTeX` 与 `XeLaTeX` 支持；
4. 使用 `tcolorbox` 宏包改写定理类环境，可跨页；
5. 定理类环境名字更新，修复定理环境交叉引用；
6. 颜色名字更新，统一链接颜色；
7. 重新绘制 ElegantLaTeX 的 Logo；
8. 更新封面与装饰物，删除水印；
9. 修正附录相关内容；
10. 增加灰色主题 `color=plain`；
11. 增加代码高亮；
12. 美化列表环境。

