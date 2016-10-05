# xsnap

Takes screenshots on Linux using `ffmpeg -f x11grab`, handling a few annoying details.
All programs take a screenshot of the current `DISPLAY` and write it to stdout.

Provides three executables:

* `xsnap-png-lossless` - outputs a true-color PNG screenshot.

* `xsnap-png-256` - outputs a 256-color PNG screenshot.  Requires [pngquant](https://github.com/pornel/pngquant) built with a libpng 1.6.

* `xsnap-jpg` - outputs a JPEG screenshot.
