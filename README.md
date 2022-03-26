# ZMK Config Optimized for Sofle Keyboards

This is a zmk config that uses a [zmk fork that is optimized for the sofle keyboard](https://github.com/infused-kim/zmk/tree/sofle). It improves encoder, display and underglow support of zmk.

While it's been optimized for and tested with a sofle choc keyboard, it can be benificial for and should work with any split keyboard that is using encoders and displays.

## It adds the following features and fixes:

* Adds underglow (used for backlight) support to Sofle shield ([PR #1188](https://github.com/zmkfirmware/zmk/pull/1188))
* Fixes split side encoder not working ([PR #728](https://github.com/zmkfirmware/zmk/pull/728))
* Fixes display not working if you toggle external power off and then on again ([Issue #674](https://github.com/zmkfirmware/zmk/issues/674))
* Adds automatic disabling and enabling of external power when USB is disconnected or connected ([PR #1184](https://github.com/zmkfirmware/zmk/pull/1184))
* Adds automatic disabling of backlight if the keyboard is idle ([PR #1179](https://github.com/zmkfirmware/zmk/pull/1179))

Most of these fixes and features have not made it into the official zmk yet, because they don't meet the (very resaonable and completely understandable) code standards of the zmk maintainers.

However, while these fixes and features may not meet the quality standards of the official project, they work well enough to be used until these features get properly implemented in the official zmk.

## How to use

1. Fork this repo
2. Clone the repo to your computer
3. Edit the config and keymap files
4. Push your changes to github
5. Download the firmware from the actions tab

Alternatively, you could probably even use github's built-in editor to edit the keymap and config file after forking.
