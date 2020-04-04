# 安装

Zettlr 的安装非常简单，在每个操作系统上都操作简单。Zettlr 是跨平台应用，因此它能够在无论哪个操作系统上运行。Zettlr 是专为 macOS、Windows 和基于 Debian, RedHat 的 Linux 系统（Ubuntu, Gnome, Xubuntu, Kubuntu, Fedora, RedHat 等）而构建的。

如果要在其他 Linux 系统（如 Arch）或 ARM 设备（如树莓）上运行 Zettlr，您必须自己创建一个包。有很多简单的教程，关于如何在网上建立 Electron 应用程序。请参阅 [Electron 应用支持的平台](https://github.com/electron/electron/blob/master/docs/tutorial/support.md)来确定最新支持的平台。

> Arch Linux 提供了一个社区维护的软件包，你可以在[官方 AUR 库](https://aur.archlinux.org/packages/zettlr-bin/)中找到。请注意，此包由社区维护，我们不对其稳定性、安全性或提供版本承担任何责任。

## Windows 7 及以上系统

要在 Windows 上安装 Zettlr，只需前往[下载页面](https://www.zettlr.com/download)并双击打开。 如果您希望为所有用户安装 Zettlr，它将安装到主 `Program Files` 文件夹中——在这种情况下，您必须在安装过程中授予其提升权限（它会自动请求您的权限）。如果您自己安装它，则不需要任何权限。

要卸载 Zettlr，只需从目录本身运行 `Uninstall.exe`，或在系统的设置中的删除选项。如果要完全删除与应用关联的所有数据，请同时删除目录 `C:\Users\<your-user-name>\AppData\Roaming\Zettlr`。

## macOS 10.10 及以上系统

要在 macOS 上安装 Zettlr，只需从最新版本下载 dmg 文件并安装它。然后，将 Zettlr 图标拖入您的应用程序目录，就完成啦！

要卸载 Zettlr，只需从应用程序目录中删除 Zettlr.app 即可。如果要完全删除与应用关联的所有数据，请同时删除目录 `/Users/<your-user-name>/Library/Application Support/Zettlr`。

> 你也可以使用 [Homebrew](https://formulae.brew.sh/cask/zettlr) 来安装 Zettlr:`$ brew cask install zettlr`

## Linux (Debian 8/Ubuntu 12.04/Fedora 21 或较新版本)

您可以通过 Linux 系统预设的的 `deb` 和 `rpm` 包。只需将软件包安装到系统上即可。

无法检测语言。请手动选择。`/home/<your-user-name>/.config/Zettlr` 文件夹。

## 软件升级

每次启动应用时，应用程序都会检查新更新。您还可以使用「帮助」菜单中的相应选项手动更新。如果有新版本可用，Zettlr 将显示一个对话框，其中包含新版本的编号、当前版本以及包含了新功能和 Bug 修复的更改日志。然后，您可以打开下载页面以下载新安装包。你可以在现有版本下直接安装，安装程序会负责删除旧版本。所有数据都将保留并迁移到新版本。

> 如果您对开发版本感兴趣，请确保在设置对话框的「进阶」选项卡中勾选复选框「通知有关测试版版本」！

## 安装 Pandoc

Zettlr 通过与一个名为 `Pandoc` 的附加软件包其他软件（如 Microsoft Word、Wiki 系统或 OpenOffice）交互。Pandoc 免费开源，它使得您能够使用 Zettlr 的所有导出和导入功能，是与其他程序及不使用 Markdown 的同事接入的理想选择。

在所有平台上安装 Pandoc 都很容易。

> 您可以随时安装 Pandoc。只需使用「应用菜单」菜单中的「帮助」项即可打开安装说明。

### Windows

在 Windows 系统中, Pandoc 可以通过访问[下载页面](https://github.com/jgm/pandoc/releases/latest)获得 Windows 安装程序。只需执行该程序，随后即可正确安装它。您可以尝试导出一点内容，如果能正常工作，就完事了！

> 请注意，由于 Pandoc 是 CLI 程序（命令行接口），因此无法显示是否有可用的更新。你必须自己进行更新：不时访问下载页面即可。

### macOS

在 macOS 中，潘多克可以通过多种方式安装。

#### 推荐使用：Homebrew

[Homebrew](https://brew.sh/)是一个很好的安装方法，Homebrew 是一个包管理器，它可以轻松地安装命令行程序（如 pandoc），并且易于维护。 请前往该页面[安装 Homebrew](https://brew.sh/)，然后只需在终端中运行以下命令：

```bash
$ brew install pandoc
```

要更新 Pandoc，请使用此命令：

```bash
$ brew upgrade
```

这将将所有已安装的公式（如调用）升级到最新版本。

> 建议使用 Homebrew 安装，因为它不仅更快，而且更方便。

设置 Pandoc 后，您可能还希望安装 `citeproc`，因为它使您能够使用 Zettlr 进行[引用](academic/citations.md)。在 Windows 上，已自动安装 Citeproc，而在 macOS 上，您必须另外安装 Pandoc Citeproc：

```bash
$ brew install pandoc-citeproc
```

#### 使用官方安装程序

要以传统方式安装 Pandoc，您只需前往[下载页面](https://github.com/jgm/pandoc/releases/latest)，即可获取 macOS 安装程序。完成后，Pandoc 在您的系统上就可用了。尝试导出一些内容，如果能正常工作，就完事了！

### Linux

On Linux, installing Pandoc is hilariously simple. Simply use your package manager to search for, and install Pandoc. The provided packages aren't always up-to-date, but they should fit. If you want to install the newest version, you'd have to [download the Linux installer](https://github.com/jgm/pandoc/releases/latest) and follow the [install instructions](https://pandoc.org/installing.html) on the Pandoc site.

> You may need to set up `pandoc-citeproc` manually by installing it using the preferred method on your operating system.

## Installing LaTeX

Markdown works best if combined with `LaTeX` to create beautiful PDF files. To do so, you'd have to install a `TeX`-distribution along Zettlr. Don't worry: You won't need to learn any `LaTeX` to use it. But you'd have to install it.

Installing the software works exactly the same as any other software: On Windows and macOS you'll need the installer package, while on Linux you can use your package manager to install a distribution.

The recommended distributions are:

- Windows: [MikTeX](https://miktex.org/download)
- macOS: [MacTex](https://www.tug.org/mactex/morepackages.html) (_Attention: It suffices to install the Basic Tex, which is much smaller than the full version!_)
- Linux: [TeX Live](https://www.tug.org/texlive/) (install the texlive-base package: `sudo apt install texlive-base`)

> You can install LaTeX at a later time. Simply use the menu item from the Help menu to open up the overview page where you can immediately see all available distributions.
