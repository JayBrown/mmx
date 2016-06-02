![mmx-platform-osx](https://img.shields.io/badge/platform-OS%20X-lightgrey.svg)
![mmx-code-shell](https://img.shields.io/badge/code-shell-yellow.svg)
[![mmx-prereq-bitbar](https://img.shields.io/badge/prerequisite-BitBar%202.0%20beta4-brightgreen.svg)](https://github.com/matryer/bitbar)
[![mmx-prereq-popclip](https://img.shields.io/badge/prerequisite-PopClip%201.5.5-brightgreen.svg)](https://github.com/matryer/bitbar)
[![mmx-depend-tnote](https://img.shields.io/badge/dependency-terminal--notifier%201.6.3-green.svg)](https://github.com/alloy/terminal-notifier)
[![mmx-license](http://img.shields.io/badge/license-MIT+-blue.svg)](https://github.com/JayBrown/mmx/blob/master/license.md)

# M.M.X
**M.M.X… for you, my lovelies… includes BitBar plugin, OS X workflow, PopClip plugin**

## Current status
v0.3.4 (stable)

Minimum OS X for full functionality: **10.10**

## Prerequisites
### Manual installations
Install into `/Applications`
* [BitBar](https://github.com/matryer/bitbar): **v2 beta4** or higher needed
* [PopClip](http://pilotmoon.com/popclip/): tested with **v1.5.5**

### Homebrew installations
Install using [Homebrew](http://brew.sh) (or with a similar manager) 
* [terminal-notifier](https://github.com/alloy/terminal-notifier): `brew install terminal-notifier`

You need to have Spotlight enabled for `mdfind` to locate the terminal-notifier.app on your volume; if you don't install terminal-notifier, or if you have deactivated Spotlight, M.M.X will call notifications via AppleScript instead

## M.M.X main installation
### Initial installation
* [Download the current release](https://github.com/JayBrown/mmx/releases); please choose the correct version, i.e. the "admin" version is, you guessed it, only for admins
* Move both main script and the subfolder including the subscripts from the DMG into your BitBar plugins directory
* Open your shell, `cd` to your BitBar plugins directory, and `chmod +x` the M.M.X script
* Double-click the .workflow file to install it into the default location `~/Library/Services`; remove any old version in case of an update
* If the workflow doesn't install on your system, try opening and re-saving it with Automator, before installing
* Double-click the .popclipext file to install the extension into PopClip, and arrange there; delete any old version in case of an update
* Launch BitBar again; it should now load M.M.X
* During load, the main script will `chmod +x` the remaining subscripts

### Subsequent installations (beginning with v0.4)
* M.M.X will notify you if an update is available
* Just click on "Update", and M.M.X will do the rest

## Future functionality (v0.4 and later)
* Subscripts for higher speed
* Drop to plugin
* Auto-update
* Change refresh rate
* Lots of minor tweaks