# xsnap

xsnap takes screenshots on Linux using `ffmpeg -f x11grab`, handling a few annoying details.
I have found that ffmpeg's x11grab is accurate, reliable, and doesn't cause any slowdowns.
It also paints the mouse cursor onto the screenshot.

Provides three executables.  All of them take a screenshot of the current `DISPLAY` and write to stdout.

* `xsnap-png-lossless` - outputs a true-color PNG screenshot.

* `xsnap-png-256` - outputs a 256-color PNG screenshot.
  Requires [pngquant](https://github.com/pornel/pngquant) built with libpng 1.6.

* `xsnap-jpg` - outputs a JPEG screenshot.


## Installation and usage

    sudo apt-get install ffmpeg x11-utils
    git clone https://github.com/ludios/xsnap
    ./xsnap/bin/xsnap-png-lossless > out.png
