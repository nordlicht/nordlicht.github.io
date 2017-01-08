---
layout: default
title: Installation
permalink: /installation/
---

## Linux

|     |     |
| --- | --- |
| Arch Linux | [`yaourt`](https://wiki.archlinux.org/index.php/Yaourt) `-S` [`nordlicht`](https://aur.archlinux.org/packages/nordlicht/) |
| Debian (stretch) | `apt-get install nordlicht`
| FreeBSD | `pkg install` [`nordlicht`](https://freshports.org/multimedia/nordlicht/) |
| Gentoo | [`layman`](https://wiki.gentoo.org/wiki/Project:Overlays/User_Guide) `-a jm-overlay && emerge -av` [`nordlicht`](http://gpo.zugaina.org/media-video/nordlicht) |
| openSUSE | `zypper install` [`nordlicht`](http://packman.links2linux.de/package/nordlicht) (from [Packman](https://en.opensuse.org/Additional_package_repositories#Packman)) |
| Ubuntu (> 16.04)| `apt-get install nordlicht` |

## Windows

You can find 32-bit Windows executables attached to the [releases](https://github.com/nordlicht/nordlicht/releases) (under *Downloads*, look for files called `nordlicht-win32-x.y.z.zip`). For starters, you can drag-and-drop videos onto the executable, this will create png files with default settings in the same directory as the video files. For advanced usage, you need to learn how to use the command line.

## Building from source

If your operating system is not listed, consider building nordlicht from source. You'll find instruction on how to do that in the README.

|     |     |
| --- | --- |
| Latest Git version | <https://github.com/nordlicht/nordlicht> |
| Stable releases | <https://github.com/nordlicht/nordlicht/releases> |
