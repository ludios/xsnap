# ffshot

Takes screenshots on Linux using `ffmpeg -f x11grab`, handling a few annoying details.

Provides three scripts:

* `lossy-png-screenshot` - outputs a 256-color PNG screenshot of the current `DISPLAY` to stdout.  Requires `pngquant` built with a libpng 1.6.

* `lossless-png-screenshot` - outputs a true-color PNG screenshot of the current `DISPLAY` to stdout.

* `lossy-jpg-screenshot` - outputs a JPEG screenshot of the current `DISPLAY` to stdout.
