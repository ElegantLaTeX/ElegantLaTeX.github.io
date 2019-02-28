---
title: Compilation Methods
description : "Compilation Methods"
weight: 1
---

This template is based on the Standard LaTeX book class, so the options of book class also work. The default encoding is UTF-8, and TeX Live is recommended. The test environment is Win10 + TeX Live 2018.

## Compile with PDFLaTeX

If you choose PDFLaTeX to process your book, the default article font computer modern has changed to `newtx` series, and the default font size is set to 12pt. The fonts are settings with:

+ `newtxtext` package for text fonts, similar to Times New Roman font.
+ `newtxmath` package for math fonts, close to `times` package.
+ `FiraMono` package for typewriter fonts, with option `scale=0.7`.
+ `ctex` package for Chinese fonts, with option `scheme=plain`.

A full compilation chain： `PDFLaTeX` -> `BibTeX` -> `PDFLaTeX`*2.

## Compile with XeLaTeX

If you choose `XeLaTeX` to process your book, we use `fontspec` package and `xeCJK` package. we used fonts available in Windows, if you are using Linux or Mac OS, please substitute these fonts with that of your system.

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
\XeTeXlinebreaklocale "zh"
\XeTeXlinebreakskip = 0pt plus 1pt minus 0.1pt
\RequirePackage{newtxmath}
```
A full compilation chain： `XeLaTeX` -> `BibTeX` -> `XeLaTeX`*2.
