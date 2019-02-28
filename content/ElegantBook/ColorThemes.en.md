---
title: Color Themes
description : "Color Themes"
weight: 3
---

This template contains 4 color themes,they are green (default), cyan, blue, plain, and there is a customization color option `nocolor`. You can choose green with

```tex
\documentclass[green]{elegantbook} %or
\documentclass[color=green]{elegantbook}
```

where plain theme is gray for all theorem class environments and paper structures. If you want to customize the colors, please select `nocolor` or use `color=none` , then define the main, second, and third colors in the preamble section as follows:

```tex
\definecolor{main}{RGB}{70,70,70}
\definecolor{second}{RGB}{115,45,2}
\definecolor{third}{RGB}{0,80,80}
```
