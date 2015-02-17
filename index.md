---
layout: default
title: nordlicht - create colorful barcodes from video files
---

> *nordlicht* is a C library for converting video files into colorful barcodes. It is inspired by the [Moviebarcode Tumblr](http://moviebarcode.tumblr.com/), but aims at the next step: Integrating these barcodes into video players to make navigation faster and more precise.
>
> *nordlicht* provides a command line tool, which you can use to generate your own barcodes easily.

## Examples

Here's the barcode for [Tears of Steel](http://tearsofsteel.org/). *nordlicht* took the movie's frames at regular intervals, scaled them them to 1 pixel width, and appended them. You can differentiate inside and outside scenes, the credits, and the "secret" scene at the end:

![](/images/tears-of-steel.png)

This barcode of [Elephants Dream](http://www.elephantsdream.org/) uses the *vertical* style, which compresses video's frames to columns and rotates them 90 degrees counterclockwise. This style emphasizes the movement of characters:

![](/images/elephants-dream-vertical.png)

## License: GPLv2+

*nordlicht* is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

The header image shows an Aurora Borealis, which is called "Nordlicht" (nord-/lɪ[ç](https://en.wikipedia.org/wiki/Voiceless_palatal_fricative)t/) in German. The picture was taken in Greenland during the [Shelios 2012 expedition](http://shelios.com/sh2012) and is available under the [Creative Commons Attribution-NonCommercial License](https://creativecommons.org/licenses/by-nc/2.0/).
