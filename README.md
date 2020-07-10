Xfce Classic Gentoo Overlay
===========================
This repository contains a gentoo overlay for some Xfce Classic packages.
Currently, libxfce4ui-nocsd is packaged.


Installation
------------
The easiest way to get started is using `eselect repository`:
```
# eselect repository add xfceclassic git https://github.com/Xfce-Classic/gentoo-overlay
# emaint sync -r xfceclassic
```

You can then install libxfce4ui-nocsd like this:
```
# emerge -av '>=libxfce4ui-4.15.3::xfceclassic'
```

Notes
-----
Currently, the libxfce4ui-nocsd package is still named xfce-base/libxfce4ui, so
when installing it, make sure emerge selects the one at ::xfceclassic. In the future
we may rename it so it exists as an independent package.
