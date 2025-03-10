Amended US keyboard with German letters and symbols as well as some Swedish letters.

![Layout](https://github.com/wasmitnetzen/keyboard/raw/main/layout.png "Layout")

## Installation

Copy the file to the appropriate location, on Ubuntu/Debian, it should be
```Bash
sudo cp custom /usr/share/X11/xkb/symbols
```

Then enable the keyboad in the input settings. It can be found as a variant of
the us layout, with my name attached.

I would recommend to enable at least one other keyboard layout as well, as a
non-functional keyboard makes it kinda hard to login in case of errors.

### KDE Plasma specific notes

Set up the layout in System Settings -> Keyboard -> Layouts (as of Plasma 6).
It caches the loaded keyboard layouts while it is running, restarting it should
be enough to make it appear.

### Home folder installation

You can put the file into `~/.config/xkb/symbols/` as well, if you don't have
root rights. There are some visual bugs around this (at least in KDE Plasma),
but it should work just as well. Most notably the preview doesn't work.

## Changes compared to American layout
* Switched y and z
* Extra letters, accessible with Level3 modifier, which is usually RAlt
  * Added German üÜ, German/Swedish äÄ, and öÖ, and Swedish åÅ to u, a, o, and p, respectively
  * Added ßẞ to s
  * Added µ to m
  * Added German quote marks „“ to ,.
  * Added section § to 4
  * Added € on 5
  * Added degree ° to 6
  * Added dead_abovering ° to CAPS+6
  * Added thin space (U2009), nobreakspace to Space bar
* Caps Lock is F24 (normal keyboard have only 12 F keys, but there's support for 24)


## Links
* https://who-t.blogspot.com/2020/09/user-specific-xkb-configuration-putting.html
* https://gitlab.freedesktop.org/xkeyboard-config/xkeyboard-config/-/issues/257

