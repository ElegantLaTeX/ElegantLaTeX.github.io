---
title: 语言模式
description : "语言模式"
weight: 2
---

本模板内含两套语言环境，改变语言环境会改变图表标题的引导词（图，表），文章结构词（比如目录，参考文献等），以及定理环境中的引导词（比如定理，引理等）。不同语言模式的启用如下：

```tex
\documentclass[cn]{elegantbook}
\documentclass[lang=cn]{elegantbook}
\documentclass[en]{elegantbook}
\documentclass[lang=en]{elegantbook}
```

__注：__ 不管选用中文环境（`lang=cn`）还是英文环境（`lang=en`）均可输入中文。另外如果在笔记中使用了抄录环境（lstlisting），并且其中包括了中文，请务必使用 `XeLaTeX` 编译。
