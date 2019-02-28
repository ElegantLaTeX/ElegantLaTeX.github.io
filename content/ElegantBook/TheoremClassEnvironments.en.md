---
title: Theorem Class Environments
description : "Theorem Class Environments"
weight: 5
---

In this template, we defined four categories of theorem class environments

+ __Theorem Environment__, including title and contents, numbering within chapter. There are three types depending on the format
    + deﬁnition environment, the color is main;
    + theorem, lemma, corollary environment, the color is second;
    + proposition environment, the color is third.
+ __Example Environments__, including example, exercise, problem environment, auto numering within chapter.
+ __Proof Environment__, including proof, note environment, they contain introductory symbol (note environment) or ending symbol (proof environment).
+ __Conclusion Environments__, including conclusion, assumption, property, remark, solution environment, all of these begin with boldfaced words, and the contents are the same as a normal paragraph.

## Theorem Class Environments

The template uses the `tcolorbox` package to customize the theorem class environments, it is slightly different from the normal theorem environments. The usage is as follows:

```tex
\begin{theorem}{<theorem name>}{<label>}
The content of theorem.
\end{theorem}
```

The ﬁrst parameter `<theorem name>` is the name of the theorem, and the second parameter `label` is the label used in cross-reference with `ref{thm:label}`. Note that cross-references must be prefixed with thm:. 

Other theorem class environments with the same usage are:

| Environment | Label text | Prefix | Cross-reference|
|-------------|--------|------|-------------------|
| definition  | label  | def  | `\ref{def:label}` | 
| theorem     | label  | thm  | `\ref{thm:label}` |
| lemma       | label  | lem  | `\ref{lem:label}` |
| corrlary    | label  | cor  | `\ref{cor:label}` |
| proposition | label  | pro  | `\ref{pro:label}` |

## Cross-reference

The other three math environments can be used directly since there are no options for them, the `example` environment usage:

```tex
\begin{example}
This is the content of example environment.
\end{example}
```

These are all the same environments, except that

+ example, exercise, problem environments numbering within chapter;
+ note with introductory symbol, proof with ending symbol;
+ conclusion environment with boldfaced keywords and normal paragraph content.
