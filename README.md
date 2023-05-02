Amended US keyboard with German letters and symbols as well as some Swedish letters.

![Layout](https://github.com/wasmitnetzen/keyboard/raw/master/layout.png "Layout")

## Installation

Apply the patches to the appropriate files, on Ubuntu, that is
```Bash
sudo patch -u -b /usr/share/X11/xkb/rules/evdev.xml -i evdev.xml.patch
sudo patch -u -b /usr/share/X11/xkb/symbols/us -i us.patch
```

The patches currently work on the files coming with Ubuntu 23.04, but should be easy to adapt to any other version. Older versions are available in the git history.

Then enable the keyboad in the input settings. It can be found as a variant of the English (US) layout. I would recommended to enable at least one other keyboard layout as well, as a non-functional keyboard makes it kinda hard to login in case of errors.

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
* Pause is Mute, Ctrl+Pause is keyboard mute

## Updating

```Bash
diff -u /usr/share/X11/xkb/rules/evdev.xml* > evdev.xml.patch
diff -u /usr/share/X11/xkb/symbols/us* > us.patch
```

## Links
* http://people.uleth.ca/~daniel.odonnell/Blog/custom-keyboard-in-linuxx11
* https://help.ubuntu.com/community/Custom%20keyboard%20layout%20definitions?action=show&redirect=Howto%3A+Custom+keyboard+layout+definitions
* https://askubuntu.com/questions/1041341/adding-multimedia-xf86-shortcut-to-regular-keys-using-xkb
* https://medium.com/@damko/a-simple-humble-but-comprehensive-guide-to-xkb-for-linux-6f1ad5e13450
