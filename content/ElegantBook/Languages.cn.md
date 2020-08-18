---
title: About Pull Request
description : "About Pull Request"
weight: 8
---

本模板内含两套语言环境，改变语言环境会改变图表标题的引导词（图，表），文章结构词（比如目录，参考文献等），以及定理环境中的引导词（比如定理，引理等）。不同语言模式的启用如下：

```tex
\documentclass[cn]{elegantbook}
\documentclass[lang=cn]{elegantbook}
```

__注：__ 只有中文环境（lang=cn）才可以输入中文。另外如果抄录环境（lstlisting）中有中文字符，请务必使用 XeLaTeX 编译。

