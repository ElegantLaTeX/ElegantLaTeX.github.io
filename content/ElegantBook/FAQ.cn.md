---
title: About Pull Request
description : "About Pull Request"
weight: 8
---

**问题**：有没有办法章节用“第一章，第一节，（一）”这种？

**答案**：你可以修改模板中对于章节的设置，利用 `ctex` 宏集的 `\zhnumber` 命令可以把计数器的数字形式转为中文。



**问题**：3.07 版本的 cls 的 `natbib` 加了`numbers` 编译完了没变化，群主设置了不可更改了？

**答案**：3.07 中在 `gbt7714` 宏包使用时，加入了 `authoryear` 选项，这个使得 `natbib` 设置了 `numbers` 也无法生效。3.08 版本中，模板增加了 `numbers` 和 `authoryear` 文献选项，你可以参考前文设置说明。



**问题**：大佬，我想把正文字体改为亮色，背景色改为黑灰色。

**答案**：页面颜色可以使用 `\pagecolor` 命令设置，文本命令可以参考[这里](https://tex.stackexchange.com/questions/278544/xcolor-what-is-the-equivalent-of-default-text-color)进行设置。



**问题**：`! LaTeX Error: Unknown option scheme=plain for package ctex.`

**答案**：你用的 CTeX 套装吧？这个里面的 `ctex` 宏包已经是已经是 10 年前的了，与本模板使用的 `ctex` 宏集有很大区别。不建议 CTeX 套装了，请卸载并安装 TeX Live 2019。



**问题**：我该使用什么版本？

**答案**：请务必使用[最新正式发行版](https://github.com/ElegantLaTeX/ElegantBook/releases)，发行版间不定期可能会有更新（修复 bug 或者改进之类），如果你在使用过程中没有遇到问题，不需要每次更新[最新版](https://github.com/ElegantLaTeX/ElegantBook/archive/master.zip)，但是在发行版更新之后，请尽可能使用最新版（发行版）！最新发行版可以在 Github 或者 TeX Live 2019 内获取。



**问题**：我该使用什么编辑器？

**答案**：你可以使用 TeX Live 2019 自带的编辑器 TeXworks 或者使用 TeXstudio，TeXworks 的自动补全，你可以参考我们的总结 [TeXworks 自动补全](https://github.com/EthanDeng/texworks-autocomplete)。推荐使用 TeX Live 2019 + TeXstudio。我自己用 VS Code 和 Sublime Text，相关的配置说明，请参考 [LaTeX 编译环境配置：Visual Studio Code 配置简介](https://github.com/EthanDeng/vscode-latex) 和 [Sublime Text 搭建 \LaTeX{} 编写环境](https://github.com/EthanDeng/sublime-text-latex)。



**问题**：您好，我们想用您的 ElegantBook 模板写一本书。关于机器学习的教材，希望获得您的授权，谢谢您的宝贵时间。

**答案**：模板的使用修改都是自由的，你们声明模板来源以及模板地址（Github 地址）即可，其他未尽事宜按照开源协议 LPPL-1.3c。做好之后，如果方便的话，可以给我们一个链接，我把你们的教材放在 ElegantLaTeX 用户作品集里。



**问题**：我想要原来的封面！

**答案**：我们计划在未来版本加入封面选择，让用户可以选择旧版封面。



**问题**：我想修改中文字体！

**答案**：首先，我们强烈建议你不要去修改字体！如果你一定坚持修改字体，请在 `newtxtext` 宏包加载前加入中文字体设置（`xeCJK` 宏包）。如果你选择自定义字体，请设置好 `\kaishu`，`\heiti` 等命令，否则会报错。如果你看不懂我现在说的，请停止你的字体自定义行为。



**问题**：请问交叉引用是什么？

**答案**：本群和本模板适合有一定 LaTeX 基础的用户使用，新手请先学习 LaTeX 的基础，理解各种概念，否则你将寸步难行。



**问题**：定义等环境中无法使用加粗命令么？

**答案**：是这样的，默认中文并没加粗命令，如果你想在定义等环境中使用加粗命令，请使用 `\heiti` 等字体命令，而不要使用 `\textbf`。或者，你可以将 `\textbf` 重新定义为 `\heiti`。英文模式不存在这个问题。



**问题**：代码高亮环境能用其他语言吗？

**答案**：可以的，ElegantBook 模板用的是 `listings` 宏包，你可以在环境之后加上语言，全局语言修改请使用 `\lstset` 命令，更多信息请参考宏包文档。



**问题**：群主，什么时候出 Beamer 的模板（主题），ElegantSlide 或者 ElegantBeamer？

**答案**：这个问题问的人比较多，我这里给个明确的答案。由于 Beamer 中有一个很优秀的主题 [Metropolis](https://github.com/matze/mtheme)。我觉得在我们找到非常好的创意之前不会发布正式的 Beamer 主题，如果你非常希望得到 ElegantLaTeX “官方”的主题，请在用户 QQ 群内下载我们测试主题 PreElegantSlide（未来不一定按照这个制作）。正式版制作计划在 2020 年之后。



**问题**：群主好棒，想嫁！

**答案**：我取向正常！