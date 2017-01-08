---
layout: default
title: nordlicht - create colorful barcodes from video files
---

> <img src="/images/nordlicht-logo.png">
> **nordlicht** is a tool that converts video files into colorful barcodes. nordlicht is free software, supports a large number of styles, and is optimized for speed. It comes with a software library written in C that allows for easy integration into other programs.

## Examples

<div class="nordlicht"><a href="/images/lion-king.png"><img src="/images/lion-king.png"></a><p>The Lion King (1994)</p></div>
<div class="nordlicht"><a href="/images/nemo.png"><img src="/images/nemo.png"></a><p>Finding Nemo (2003)</p></div>
<div class="nordlicht"><a href="/images/titanic.png"><img src="/images/titanic.png"></a><p>Titanic (1997)</p></div>

Even if you don't know the movies, you can probably spot the fire scene in The Lion King, the dirty fish tank scene in Finding Nemo, and the sinking scene in Titanic. You can also see the credits, and spot outdoor scenes (which feature a blue sky in the upper half).

nordlicht creates these images by taking the movies' frames in regular intervals, scaling them to 1 pixel width, and putting them next to each other.

## Styles

The default style is **horizontal**, which compresses each frame to a single column before appending them. This style emphasizes landscapes and up-and-down movement. Also, it is usually the best style for differentiating scenes:

<div class="nordlicht"><a href="/images/cosmos-horizontal.png"><img src="/images/cosmos-horizontal.png"></a><p>Cosmos Laundromat (2015), <b>horizontal</b></p></div>

The **vertical** style, on the other hand, compresses each individual frames to a single row, rotates them counterclockwise by 90 degrees, and then sticks them together. This style emphazizes horizontal movement and sometimes lets you recognize objects or characters standing next to each other:

<div class="nordlicht"><a href="/images/cosmos-vertical.png"><img src="/images/cosmos-vertical.png"></a><p>Cosmos Laundromat (2015), <b>vertical</b></p></div>

The simple **thumbnails** style just creates a row of thumbnails as you would expect:

<div class="nordlicht"><a href="/images/cosmos-thumbnails.png"><img src="/images/cosmos-thumbnails.png"></a><p>Cosmos Laundromat (2015), <b>thumbnails</b></p></div>

When using the **middlecolumn** style, nordlicht will not compress the frames, but just go with the middlemost column of each frame. This is like watching the movie through a thin crack. It highlights colors and texture in the center of the screen, and can result in interesting effects when the camera is moving sideways:

<div class="nordlicht"><a href="/images/cosmos-middlecolumn.png"><img src="/images/cosmos-middlecolumn.png"></a><p>Cosmos Laundromat (2015), <b>middlecolumn</b></p></div>

The **slitscan** style works in a similar way, but instead of always selecting the middle column, the selected column is moved over the width of the video from left to right, so that one pass takes as long as one frame in the *thumbnails* style. Think of it as watching the movie through a thin, *moving* crack. This style is interesting because for long, static scenes, parts of the content becomes recognizable while still maintaining accuracy:

<div class="nordlicht"><a href="/images/cosmos-slitscan.png"><img src="/images/cosmos-slitscan.png"></a><p>Cosmos Laundromat (2015), <b>slitscan</b></p></div>

Finally, the **spectrogram** style is different from all previous styles because it analyzes the file's audio track and creates a *spectrogram*: Low frequencies are at the bottom, high frequencies at the top, and the color describes the volume of that frequency (warmer colors means higher volume):

<div class="nordlicht"><a href="/images/cosmos-spectrogram.png"><img src="/images/cosmos-spectrogram.png"></a><p>Cosmos Laundromat (2015), <b>spectrogram</b></p></div>

For convenience, nordlicht also supports putting multiple styles in the same image. For example, this is the resulting image for the style **slitscan+spectrogram**:

<div class="nordlicht"><a href="/images/cosmos-slitscan+spectrogram.png"><img src="/images/cosmos-slitscan+spectrogram.png"></a><p>Cosmos Laundromat (2015), <b>slitscan+spectrogram</b></p></div>

## What's next?

If you're interested, you can learn how to [install](/installation/) and [use](/usage/) nordlicht.

## License: GPLv2+

*nordlicht* is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

The header image shows an aurora borealis, which is called "Nordlicht" (nord-/lɪ[ç](https://en.wikipedia.org/wiki/Voiceless_palatal_fricative)t/) in German. The picture was taken in Greenland during the [Shelios 2012 expedition](http://shelios.com/sh2012) and is available under the [Creative Commons Attribution-NonCommercial License](https://creativecommons.org/licenses/by-nc/2.0/).
