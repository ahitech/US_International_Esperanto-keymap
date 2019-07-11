# US_International_Esperanto-keymap
Keymap for Haiku OS that supports special Esperanto characters via "dead-keys"

## Description

Esperanto is the most successful planned international language in the world.
[Haiku operating system](https://www.haiku-os.org) already supports Esperanto
as an input method. However, since English is much more useful, switching
between Esperanto and US International keymaps for the few special Esperanto
characters is not practical.

Therefore here is the unified English-Esperanto keymap.

## Installation

1. Install Keymap Switcher:
   - [For x86_84](https://depot.haiku-os.org/#!/pkg/keymapswitcher/haikuports/1/2/7.11/-/8/x86_64)
   - [For x86 32-bits](https://depot.haiku-os.org/#!/pkg/keymapswitcher/haikuports/1/2/7.11/-/8/x86_gcc2)
   
   Note: these links are leading to a specific version. You may want to check [Haiku Depot](https://depot.haiku-os.org)
   and see if there is a newer version for your architecture.
   
2. Download the file US_International_Esperanto from this repository into ~/config/settings/Keymap

3. In Keymap Switcher preferences, find the "US_International_Esperanto" keymap in the
   "Available keymaps" list, at the bottom, (in the list of user-defined keymaps), and 
   drag this keymap into the top list "Selected keymaps", arranging it to your preference
   with or without other keymaps.
   
## Using

This keymap works exactly like the system-provided "US International 104-keys" keymap, but
it has Esperanto characters hooked onto keyboard dead keys.

Dead key does not print a character, instead it modifies the following character.

I have replaced all keys modified by the [circumflex](https://en.wikipedia.org/wiki/Circumflex)
dead key with the Esperanto characters. **This keymap does not support other characters with circumflex**,
only Esperanto ones. 

| To type | Press                                 |
| ------- | ------------------------------------- |
|  Ĉ or ĉ | `Option`+`Shift`+`^`, then `C` or `c` |
|  Ĝ or ĝ | `Option`+`Shift`+`^`, then `G` or `g` |
|  Ĥ or ĥ | `Option`+`Shift`+`^`, then `H` or `h` |
|  Ĵ or ĵ | `Option`+`Shift`+`^`, then `J` or `j` |
|  Ŝ or ŝ | `Option`+`Shift`+`^`, then `S` or `s` |
|  Ŭ or ŭ | `Option`+`Shift`+`^`, then `U` or `u` |

**Note**: by default, `Option` key is `Windows` key. Instead of `Option`, you can use `AltGr` key, which is right `Alt`.

## Modifying

1. Open `Terminal`.
2. Issue the following command: `keymap -o ~/US_International_Esperanto_Modified -d ~/config/settings/Keymap/US_International_Esperanto`
3. Edit the file `~/US_International_Esperanto_Modified` with the text editor of your choise.
4. Save the changes :WINK:
5. Issue the following command: keymap -c ~/US_International_Esperanto_Modified -o ~/config/settings/Keymap/US_International_Esperanto_Modified`
6. Select the new `US_International_Esperanto_Modified` keymap in the Keymap Switcher, as described above.

## Uninstallation

1. Remove the keymap from the Keymap Switcher list of "Selected keymaps".
2. Remove the file ~/config/settings/Keymap/US_International_Esperanto

## That's all folks!

Have fun!
