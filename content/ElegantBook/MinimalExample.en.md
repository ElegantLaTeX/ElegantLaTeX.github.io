---
title: Minimal Example
description : "Minimal Example"
weight: 10
---

Here is a minimal example.

```tex
\documentclass{elegantbook}

% title info
\title{Title}
\subtitle{Subtitle is here}

% bio info
\author{Your Name}
\institute{XXX University}
\date{\today}

% extra info
\version{1.00}
\equote{Victory won\rq t come to us unless we go to it. --- M. Moore}
\logo{logo.png}
\cover{cover.jpg}

\begin{document}

\maketitle
\tableofcontents
\mainmatter
\hypersetup{pageanchor=true}

% add preface chapter here if needed
\chapter{Example Chapter Title}
The content of chapter one.

\bibliography{reference}
\appendix

\chapter{Appendix Chapter Title}
The content of appendix 1.

\end{document}
```
