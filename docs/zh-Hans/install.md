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

## Linux (Debian 8/Ubuntu 12.04/Fedora 21 或更新版本)

您可以通过 Linux 系统预设的的 `deb` 和 `rpm` 包。只需将软件包安装到系统上即可。

无法检测语言。请手动选择。`/home/<your-user-name>/.config/Zettlr` 文件夹。

## Updating the app

The application checks for new updates each time you start the app. You can also manually trigger the search for updates by using the respective menu item from the Help-menu. If there is a new version available, Zettlr will show you a dialog that contains both the new version's number, your current version and a changelog with all features and bug fixes the new version contains. You can then open the download page to download the new package. Simply install it over your current installation, it will take care of removing the old version first. All data will be retained and migrated to the new version.

> If you are interested in cutting-edge releases, make sure to tick the checkbox "Notify me about beta releases" in the advanced tab of the preferences dialog!

## Installing Pandoc

What makes Zettlr interact with other software such as Microsoft Word, Wiki-systems or OpenOffice is an additional software package called `Pandoc`. Pandoc is free and Open Source and it allows you to use all exporting and importing features of Zettlr, making it the ideal choice to be the interface between other programs and co-workers who do not use Markdown.

Installing Pandoc is easy on all platforms.

> You can install Pandoc at any time. Simply use the menu item from the Help menu to open up the installation instructions.

### Windows

On Windows, Pandoc can be installed by visiting the [download page](https://github.com/jgm/pandoc/releases/latest) and retrieving the Windows installer. Simply execute it. Afterwards, it should be installed correctly. Try to export something. If it works, you're done!

> Please note that due to the fact that Pandoc is a CLI-program (Command Line Interface), it cannot show you whether or not there is an update available. You'll have to do this yourself. Simply visit the download page from time to time.

### macOS

On macOS, Pandoc can be installed in a variety of ways.

#### Recommended method: Homebrew

The preferred method is [Homebrew](https://brew.sh/). Homebrew is a package manager that makes it easy to install command line programs such as pandoc and makes it easy to maintain it. Make sure to [install Homebrew](https://brew.sh/), and then simply run the following command in the Terminal:

```bash
$ brew install pandoc
```

To update pandoc from time to time, use this command:

```bash
$ brew upgrade
```

This will upgrade all installed formulae (as they are called) to the newest version.

> Installing with Homebrew is recommended, as it is not only faster, but also more convenient.

After pandoc is set up, you may want to install `citeproc` as well, as it provides you with the ability to [cite](academic/citations.md) using Zettlr. On Windows, Citeproc is automatically installed, while on macOS you will have to install Pandoc Citeproc additionally. Simply use Homebrew for this as well:

```bash
$ brew install pandoc-citeproc
```

#### Install using the official installer

To install Pandoc the old way, simply head over to the [download page](https://github.com/jgm/pandoc/releases/latest) and get the macOS installer. Once it is done, pandoc should be available on your system. Try to export something. If it works, you're done!

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
