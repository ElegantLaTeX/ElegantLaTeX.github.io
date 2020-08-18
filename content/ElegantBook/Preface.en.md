If you want to add a preface before the first chapter with the number of chapter unchanged, please add the preface in the following way:

```tex
\chapter*{Preface}
\addcontentsline{toc}{chapter}{Preface}
\markboth{Preface}{}
The content of Preface.
```
