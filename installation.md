---
layout: default
title: Installation
permalink: /installation/
---

There are packages for some Linux distributions:

- Arch Linux: Install [`nordlicht`](https://aur.archlinux.org/packages/nordlicht/) from the [AUR](https://wiki.archlinux.org/index.php/Arch_User_Repository)
- Gentoo: Install `media-video/nordlicht` from the *multimedia* [overlay](https://www.gentoo.org/proj/en/overlays/userguide.xml)
- openSUSE: Install [`nordlicht`](http://packman.links2linux.de/package/nordlicht) from [Packman](http://en.opensuse.org/Additional_package_repositories#Packman)'s *Multimedia* project
- Ubuntu: Install `nordlicht` from Launchpad's [ppa:blinry/nordlicht](https://launchpad.net/~blinry/+archive/nordlicht), [here's how](https://help.launchpad.net/Packaging/PPA/InstallingSoftware)

On other operating systems, get CMake, FFmpeg/libav, libpng, [popt](http://freecode.com/projects/popt), and [help2man](https://www.gnu.org/software/help2man/), and issue: `cmake .. && make` to create the `nordlicht` binary. Consider [contributing](#contributing) a package!
