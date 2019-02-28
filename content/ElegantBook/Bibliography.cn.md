---
title: 参考文献
description : "参考文献"
weight: 8
---

此模板使用了 `BibTeX` 来生成参考文献，默认使用的文献样式（bib style）是 `aer`。参考文献示例：Chen et al. (2018) 使用了中国一个大型的 P2P 平台（人人贷）的数据来检验男性投资者和女性投资者在投资表现上是否有显著差异。

你可以在谷歌学术，Mendeley，Endnote 中获得文献条目（bib item），然后把它们添加到 `reference.bib` 中。在文中引用的时候，引用它们的键值（bib key）即可。注意需要在编译的过程中添加 `BibTeX` 编译。如果你想在参考文献中添加未引用的文献，可以使用

```tex
\nocite{EINAV2010,Havrylchyk2018} 
```
