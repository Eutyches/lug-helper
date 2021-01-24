# LUG-Helper
**Star Citizen's Linux Users Group Helper Script**

https://robertsspaceindustries.com/orgs/LUG

*Greetings, fellow Penguin!*

This script is designed to help you manage and optimize Star Citizen on Linux.

Zenity menus are used for a GUI experience with a fallback to terminal-based menus where Zenity is unavailable. The game directory paths provided by the user on first run are saved in *$XDG_CONFIG_HOME/starcitizen-lug*.  Keybinds are backed up to *$XDG_CONFIG_HOME/starcitizen-lug/keybinds*

## Options:

`Preflight Check`
- Run a series of system optimization checks and offer to fix any issues.
  - Checks that vm.max_map_count is set to at least 16777216 to give the game access to sufficient memory.
  - Checks that the hard open file descriptors limit is set to at least 524288.

`Manage Lutris Runners`
- Quickly install and delete Lutris wine runners

`Delete my Star Citizen USER folder and preserve my keybinds`
- The helper will make backups of any exported keybinds, delete your Star Citizen USER folder, then restore your keybind files.
- To export your keybinds from within the game, go to:
  - *Options->Keybindings->Control Profiles->Save Control Settings*
- To re-import your keybinds from within the game, select them from the list:
  - *Options->Keybindings->Control Profiles*

`Delete my shaders only`
- Sometimes all you need to do between major version updates is delete your shaders directory.

`Delete my DXVK cache`
- A troubleshooting step that sometimes helps fix various issues and crashes.

`Get a random Penguin's Star Citizen referral code`
- Display a referral code for a random member of the Star Citizen Linux Users Group.

`Switch the helper between LIVE and PTU`
- Toggle between targeting LIVE or PTU for all of the above options.  Defaults to LIVE on each run.

## Installation:

From Source:
1. Download it!
2. Run it!
3. If you want, move *lug-logo.png* to */usr/share/pixmaps/*

Arch Linux: https://aur.archlinux.org/packages/lug-helper/

## Contributors:
- https://github.com/Termuellinator
- https://github.com/pstn
- Runner Downloader inspired by https://github.com/richardtatum/sc-runner-updater
