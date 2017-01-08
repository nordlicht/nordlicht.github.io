---
layout: default
title: Installation
permalink: /installation/
---

For some operating systems, there are already packages. For others, consider building nordlicht from source, see below.

## Packages

|     |     |
| --- | --- |
| Arch Linux | [`yaourt`](https://wiki.archlinux.org/index.php/Yaourt) `-S` [`nordlicht`](https://aur.archlinux.org/packages/nordlicht/) |
| Debian (stretch) | `apt-get install nordlicht`
|                  | `apt-get install libnordlicht-dev`|
| FreeBSD | `pkg install` [`nordlicht`](https://freshports.org/multimedia/nordlicht/) |
| Gentoo | [`layman`](https://wiki.gentoo.org/wiki/Project:Overlays/User_Guide) `-a jm-overlay && emerge -av` [`nordlicht`](http://gpo.zugaina.org/media-video/nordlicht) |
| openSUSE | `zypper install` [`nordlicht`](http://packman.links2linux.de/package/nordlicht) (from [Packman](https://en.opensuse.org/Additional_package_repositories#Packman)) |
| Ubuntu (> 16.04)| `apt-get install nordlicht` |
|                 | `apt-get intall libnordlicht-dev` |

## Windows

You can find 32-bit Windows executables attached to the [releases](https://github.com/nordlicht/nordlicht/releases) (under *Downloads*, look for files called `nordlicht-win32-x.y.z.zip`).

## Building from source

You'll find instruction on how to build nordlicht from source in the README.

|     |     |
| --- | --- |
| Latest Git version | <https://github.com/nordlicht/nordlicht> |
| Stable releases | <https://github.com/nordlicht/nordlicht/releases> |
