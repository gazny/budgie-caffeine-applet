# Budgie Caffeine Applet

Simple applet to prevent screen dimming on long idle time.

![The applet](https://raw.githubusercontent.com/yursan9/budgie-caffeine-applet/master/img/initial-applet.png)

## Feature

- Prevent screen dimming
- Prevent triggering lock screen
- Notification support (For you who want visual noise)

![notification support](https://raw.githubusercontent.com/yursan9/budgie-caffeine-applet/master/img/notification-support.png)

## Requirement

- gtk3
- gobject-introspection
- python3
- meson >= 0.40
- ninja
- python-gobject
- libnotify (notify-send)
- budgie-1.0 >= 2

## Installation

**ONLY TESTED** on fully updated Solus with Budgie 10.4

To install this applet, follow instruction below:
```
git clone https://github.com/yursan9/budgie-caffeine-applet
cd budgie-caffeine-applet
meson builddir --prefix=/usr
cd builddir
```

After that, we'll install the applet with command below
```
sudo ninja install
```

If you want to remove the applet, use `sudo ninja uninstall`.

## Issue

Only `papirus` icon theme support the icons used by this applet. Because of
that, I provided some ugly fallback icon for you. If you think you can make
better icons, I'll merge your PR.

If any other issues arise, let me know!

*Salam kopi!*
