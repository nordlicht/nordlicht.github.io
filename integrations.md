---
layout: default
title: Video Player Integrations
permalink: /integrations/
---

nordlicht is inspired by the [Moviebarcode Tumblr](http://moviebarcode.tumblr.com/), but aims at the next step: Integrating these timebars into video players to make navigation faster and more precise.

To put it differently – why do we use this...

![](/images/vlc-before.png)

When we *could* have this?

![](/images/vlc-after.png)

## mpv

For the (awesome!) [mpv](http://mpv.io/) (>= 0.3.6), there is an experimental [lua plugin](http://github.com/nordlicht/nordlicht/blob/master/utils/mpv-nordlicht.lua). Symlink the file from `~/.mpv/scripts/`, and mpv displays a live-updating timebar of the current video file at the top. You can turn it on and off by pressing `n`. You'll need ImageMagick! This is how it looks like (for [Decay](http://www.decayfilm.com/)):

![](/images/mpv-integration.png)

For mpv >= 0.2.0, there is an older script called [mpv-nordlicht](http://github.com/nordlicht/nordlicht/blob/master/utils/mpv-nordlicht). Put it in your `PATH` and use it instead of `mpv`. It doesn't support multiple files, and you cannot hide the timebar.

## GNOME file thumbnails

Copy or hardlink [this file](https://github.com/nordlicht/nordlicht/blob/master/utils/nordlicht.thumbnailer) to `/usr/share/thumbnailers` to enable nordlicht thumbnails of video files in GNOME applications. Note that generation might take a long time, depending on the length and resolution of your videos:

![](/images/nautilus-integration.png)
