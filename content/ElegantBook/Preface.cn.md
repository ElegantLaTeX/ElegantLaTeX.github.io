---
title: 序章
description : "序章"
weight: 9
---

如果你想在第一章前面添加序章，不改变原本章节序号，你可以在第一章内容前面使用

```tex
\chapter*{序章}
\addcontentsline{toc}{chapter}{序章}
\markboth{序章}{}
序章的内容。
```
