---
title: Preface
description : "Preface"
weight: 9
---

If you want to add a preface before the first chapter without changing the number of chapter, you can use it before the first chapter

```tex
\chapter*{Preface}
\addcontentsline{toc}{chapter}{Preface}
\markboth{Preface}{}
The content of Preface.
```
