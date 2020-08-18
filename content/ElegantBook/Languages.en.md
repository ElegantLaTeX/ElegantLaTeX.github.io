---
title: About Pull Request
description : "About Pull Request"
weight: 8
---

We deﬁned one option named `lang`, this option has two alternative values, `lang=en` (default) or `lang=cn`. Different values will alter the captions of figure/table, abstract name, refname, etc. You can use this option as

```tex
\documentclass[lang=cn]{elegantbook}
\documentclass[lang=en]{elegantbook}
```

__Remark__: Chinese Characters  are acceptable whenever `lang=en` or `lang=cn`. If you would like to include Chinese characters under (`lstlisting`) environment, please use `XeLaTeX` to compile.

