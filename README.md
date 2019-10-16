Amended US keyboard with German letters and symbols as well as some Swedish letters.

![Layout](https://github.com/wasmitnetzen/keyboard/raw/master/layout.png "Layout")

## Installation
On Ubuntu, copy the `us` file to `/usr/share/X11/xkb/symbols/` and `evdev.xml` to `/usr/share/X11/xkb/rules/`. It is recommended to backup the original files before and also enable another keyboard layout, as a non-functional keyboard makes it kinda hard to login.

## Changes to American layout
* Switched y and z
* Extra letters, accessible with Level3 modifier, which is usually RAlt
  * Added German äÄ, üÜ and German/Swedish öÖ to a, u, and o, respectively
  * Added ßẞ to s
  * Added µ to m
  * Added German quote marks „“ to ,.
  * Added section § to 4
  * Added € on 5
  * Added degree ° to 6
  * Added dead_abovering ° to CAPS+6 to be able to produce åÅ
  * Added thin space (U2009), nobreakspace to Space bar
* Pause is Mute
* TODO: add aring, Aring (but where? a is already used)

## Links
* http://people.uleth.ca/~daniel.odonnell/Blog/custom-keyboard-in-linuxx11
* https://help.ubuntu.com/community/Custom%20keyboard%20layout%20definitions?action=show&redirect=Howto%3A+Custom+keyboard+layout+definitions
* https://askubuntu.com/questions/1041341/adding-multimedia-xf86-shortcut-to-regular-keys-using-xkb
* https://medium.com/@damko/a-simple-humble-but-comprehensive-guide-to-xkb-for-linux-6f1ad5e13450
