---
title: About Pull Request
description : "About Pull Request"
weight: 8
---

本节介绍如何通过免安装或者安装模板（包）方式使用。

### 免安装方式安装

从 Github 或者 CTAN 下载最新（正式）版文件，严格意义上只需要类文件 `elegantbook.cls`。然后将模板文件放在你的工作目录下即可使用。这样使用的好处是，无需安装，简便；缺点是，当模板进行更新之后，你需要手动替换。

### 安装模板方式安装

如果你是 TeX Live 2019 用户，我们非常推荐你直接进行安装和更新。你可以通过 TeX Live 2019 自带的tlshell进行安装。安装非常简单，步骤如下，搜索并打开 tlshell，然后通过 `File -> Load Default Repository` 加载远程仓库，如果你不想使用默认的仓库，你可以通过 Options 下的菜单设置远程仓库。设置好仓库之后，等待仓库加载完毕，你可以在下面的搜索栏搜索 elegantbook，然后选择进行安装与更新。

![](https://raw.githubusercontent.com/wiki/izinngo/public/image/tlshell.png)

如果你是 TeX Live 2018 的用户，由于 2018 无法更新到 2019，所以你想更新的话，需要卸载 2018 重装 2019。如果你实在不想折腾，那么你仍然可以使用本模板，你可以手动安装模板，将elegantbook.cls复制到你的 TeXLive 目录下，默认安装目录为 `C:\texlive\2019\texmf-dist\tex\latex\elegantbook`，然后通过命令行（管理员权限），运行 texhash 即可。

啥？你是 CTeX 用户？Sorry，本模板不提供支持。

更多关于 TeX Live 2019 的安装使用以及 CTeX 与 TeX Live 的兼容、系统路径问题，请参考官方文档以及啸行的[一份简短的安装 LaTeX的介绍](https://github.com/OsbertWang/install_latex/releases)。

### 在线使用模板

考虑到用户的在线合作需求，我们把三套模板全部上传到 [Overleaf](https://www.overleaf.com/) 上了，网络通畅的用户可以直接通过 Overleaf 在线使用我们的模板。这样的好处是无需安装 TeX Live 2019，可以随时随地访问自己的文件。查找模板，请在 Overleaf 模板库里面搜索 elegantlatex 即可，你也可以直接访问[搜索结果](https://www.overleaf.com/latex/templates?addsearch=elegantlatex)。选择适当的模板之后，将其Open as Template，即可把模板存到自己账户下，然后可以自由编辑以及与别人一起协作。更多关于 Overleaf 的介绍和使用，请参考 Overleaf 的[官方文档](https://www.overleaf.com/learn)。

**注**：Overleaf 上，中文需要使用 XeLaTeX 进行编译，英文可以使用 PDFLaTeX 与 XeLaTeX 进行编译。

