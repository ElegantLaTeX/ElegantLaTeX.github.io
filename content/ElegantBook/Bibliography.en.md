---
title: Bibliography
description : "Bibliography"
weight: 8
---

This template uses `BibTeX` to generate the bibliography, the default bibliography style is `aer`. 

If you want to use `BibTeX`, you must create a file named `reference.bib`, add bib items (from Google Scholar, Mendeley, EndNote, and etc.) to `reference.bib` file, then cite the bib key in the `tex` file. The `BibTeX` will automatically generate the bibliography for the reference you cited. If you want to add some non-cited reference to the bibliography, you can use 

```tex
\nocite{EINAV2010,Havrylchyk2018} %or include some bibitems
\nocite{*} %include all the bibitems
```

Two more options `cite=numbers` and `cite=authoryear` are available in this new version, with the default setting as `numbers` since those major in science and technology use `numbers` more often. For those who major in liberal arts want to use `authoryear`, please type in:

```tex
\documentclass[cite=authoryear]{elegantbook} %or
\documentclass[authoryear]{elegantbook}
```

