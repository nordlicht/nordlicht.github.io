---
layout: default
title: Usage
permalink: /usage/
---

## Command line tool

Basic usage: `nordlicht video.mp4` converts *video.mp4* to a *horizontal*-style barcode and writes it to *video.mp4.nordlicht.png*. You can find descriptions of the different styles [on the front page](/).

Run `nordlicht --help` to see the advanced options:

    Usage: nordlicht [OPTION]... VIDEOFILE

    Options:
      -w, --width=INT           set the barcode's width; by default it's
                                "height*10", or 1920 pixels, if both are undefined
      -h, --height=INT          set the barcode's height; by default it's
                                "width/10"
      -o, --output=FILENAME     set output filename, the default is VIDEOFILE.png;
                                when you specify an *.bgra file, you'll get a raw
                                32-bit BGRA file that is updated as the barcode is
                                generated
      -s, --style=STYLE         default is 'horizontal', see "Styles" section
                                below. You can specify more than one style,
                                separated by '+', to get multiple tracks
          --start=FLOAT         specify where to start the barcode (ratio between
                                0 and 1)
          --end=FLOAT           specify where to end the barcode (ratio between 0
                                and 1)
      -q, --quiet               don't show progress indicator
          --help                display this help and exit
          --version             output version information and exit

    Styles:
      horizontal     compress frames to vertical lines and append them
      vertical       compress frames to horizontal lines and rotate them
                     counterclockwise by 90 degrees
      slitscan       take single columns while constantly moving to the right
                     (and wrapping back to the left)
      middlecolumn   take the middlemost column of each frame
      thumbnails     display small thumbnails at regular intervals
      spectrogram    spectrogram of the first audio track (not all sample formats
                     are supported yet)

    Examples:
      nordlicht video.mp4
          generate video.mp4.nordlicht.png of default size
      nordlicht video.mp4 -s vertical
          compress individual frames to columns
      nordlicht video.mp4 -w 1000 -h 1000 -o barcode.png
          override size and name of the output file

## Library

- API documentation: see [nordlicht.h](http://github.com/nordlicht/nordlicht/blob/master/src/nordlicht.h)
- Usage example: see [main.c](http://github.com/nordlicht/nordlicht/blob/master/src/main.c) (look for "interesting stuff begins here!" :-)
