---
title: 定理类环境
description : "定理类环境"
weight: 5
---

在我们这个模板中，定义了四大类环境

+ __定理类环境__：包含标题和内容两部分，全部定理类环境的编号均以章节编号。根据格式的不同分为 3 种
    + definition 环境，颜色为 main；
    + theorem、lemma、corollary 环境，颜色为 second；
    + proposition 环境，颜色为 third。
+ __示例类环境__：有 example、exercise、problem 环境（对应于例，练习，例题），自动编号，编号以章节为单位。
+ __证明类环境__：，有 proof、note 环境，特点是，有引导符或者结尾符，note 环境有引导符号，proof 环境有证明完毕符号。
+ __结论类环境__：有 conclusion、assumption、property，remark、solution 环境，三者均以粗体的引导词为开头，和普通段落格式一致。

__评论：__ 在选用 `lang=cn` 时，定理类环境的引导词全部会改为中文。

##  定理类环境的使用

由于本模板使用了 tcolorbox 宏包来定制定理类环境，所以和普通的定理环境的使用有些许区别，定理的使用方法如下：

```tex
\begin{theorem}{<theorem name>}{<label>}
The content of theorem.
\end{theorem}
```

第一个必选项 `<theorem name>` 是定理的名字，第二个必选项 `<label>` 是交叉引
用时所用到的标签，交叉引用的方法为 `\ref{thm:label}`。请注意，交叉引用时必
须加上前缀 `thm`:。其他相同用法的定理类环境有：

| 环境名       | 标签名  | 前缀  | 交叉引用            |
|-------------|--------|------|-------------------|
| definition  | label  | def  | `\ref{def:label}` | 
| theorem     | label  | thm  | `\ref{thm:label}` |
| lemma       | label  | lem  | `\ref{lem:label}` |
| corrlary    | label  | cor  | `\ref{cor:label}` |
| proposition | label  | pro  | `\ref{pro:label}` |

## 其他数学环境的使用

其他三种数学环境因为没有选项，可以直接使用，比如 example 环境

```tex
\begin{example}
This is the content of example environment.
\end{example}
```

这几个都是同一类环境，区别在于

+ 示例环境（`example`）、练习（`exercise`）与例题（`problem`）章节自动编号；
+ 注意（`note`）环境有提醒引导符，证明（`proof`）环境有证明结束符；
+ 结论（`conclusion`）等环境都是普通段落环境，引导词加粗。

