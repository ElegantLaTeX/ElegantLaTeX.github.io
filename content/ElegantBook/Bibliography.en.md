---
title: Bibliography
description : "Bibliography"
weight: 8
---

This template uses `BibTeX` to generate the bibliography, the default bibliography style is `aer`. Let’s take a glance at the citation effect, Chen et al. (2018) use data from a major peer-to-peer lending marketplace in China to study whether female and male investors evaluate loan performance differently.

If you want to use BibTeX, you must create a file named `reference.bib`, and add bib items (from Google Scholar, Mendeley, EndNote, and etc.) to `reference.bib` file, and cite the bibkey in the `tex` ﬁle. The `BibTeX` will automatically generate the bibliography for you for the reference you cited. If you want to add some noncited reference to the bibliography, you can use

```tex
\nocite{EINAV2010, Havrylchyk2018}
```
