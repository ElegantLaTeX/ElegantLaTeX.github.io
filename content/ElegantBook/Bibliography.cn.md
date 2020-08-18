此模板使用了 BibTeX 来生成参考文献，在中文示例中，使用了 gbt7714 宏包。参考文献示例：[1-3] 使用了中国一个大型的 P2P 平台（人人贷）的数据来检验男性投资者和女性投资者在投资表现上是否有显著差异。

你可以在谷歌学术，Mendeley，Endnote 中获得文献条目（bib item），然后把它们添加到 `reference.bib` 中。在文中引用的时候，引用它们的键值（bib key）即可。注意需要在编译的过程中添加 `BibTeX` 编译。如果你想在参考文献中添加未引用的文献，可以使用

```tex
\nocite{EINAV2010,Havrylchyk2018} %or include some bibitems
\nocite{*} %include all the bibitems
```

本模板还添加了 `cite=numbers` 和 `cite=authoryear` 两个参考文献选项，用于设置参考文献格式的设置，默认为 numbers。据我们所知，理工科类一般使用 numbers，而文科类使用 authoryear 比较多，所以我们将 numbers 作为默认格式。如果需要改为 authoryear，可以使用

```tex
\documentclass[cite=authoryear]{elegantbook} %or
\documentclass[authoryear]{elegantbook}
```

