---
title: Languages
description : "Languages"
weight: 2
---

We deﬁned one option named `lang`, this option has two alternative values, `lang=en` (default) or `lang=cn`. `lang=cn` will make the caption of ﬁgure/table, abstract name, refname etc. Chinese, while `lang=en` will keep all these stuff English, as the default article class sets. You can use this option as

```tex
\documentclass[cn]{elegantbook}
\documentclass[lang=cn]{elegantbook}
\documentclass[en]{elegantbook}
\documentclass[lang=en]{elegantbook}
```

__Remark__: You can input Chinese Character in either `lang=en` or `lang=cn`. If you are using (lstlisting) environment, and it contains Chinese characters, please use `XeLaTeX`.
