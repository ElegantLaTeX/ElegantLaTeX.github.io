如果你想在第一章前面添加序章，不改变原本章节序号，你可以在第一章内容前面使用

```tex
\chapter*{Introduction}
\addcontentsline{toc}{chapter}{Introduction} 
\markboth{Introduction}{} 
The content of introduction.
```

