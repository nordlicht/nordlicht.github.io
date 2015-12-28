---
layout: default
title: Video Player Integrations
permalink: /integrations/
---

nordlicht is inspired by the [Moviebarcode Tumblr](http://moviebarcode.tumblr.com/), but aims at the next step: Integrating these barcodes into video players to make navigation faster and more precise.

## mpv

For [mpv](http://mpv.io/) (>= 0.3.6), there is an experimental [lua plugin](http://github.com/nordlicht/nordlicht/blob/master/utils/mpv-nordlicht.lua). Symlink the file from `~/.mpv/scripts/`, and mpv displays a live-updating barcode of the current video file at the top. You can turn it on and off by pressing `n`. You'll need ImageMagick! This is how it looks like (for [Decay](http://www.decayfilm.com/)):

![](/images/mpv-integration.png)

For mpv >= 0.2.0, there is an older script called [mpv-nordlicht](http://github.com/nordlicht/nordlicht/blob/master/utils/mpv-nordlicht). Put it in your `PATH` and use it instead of `mpv`. It doesn't support multiple files, and you cannot hide the barcode.
