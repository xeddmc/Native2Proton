# Native2Proton

Native2Proton is a runner for forcing the install and execution of Windows versions of Steam games rather than running the native Linux version.

Requires python3

# Using Native2Proton

To clone the repo: 

```git clone https://github.com/Holston5/Native2Proton.git && cd Native2Proton```

Run with `./native2proton.py`

The Steam ID for the game you wish to install is required.  It can be found in the url of the steam store page for the game.

Detection of your steam install location should be automatic and Native2Proton also includes a wrapper for running winetricks on the prefixes it creates.

# Running Native2Proton Games

Games installed with Native2Proton are best added to your Steam client as a non-Steam game.
To do this point Steam to the .desktop shortcut created in "~/.local/share/native2proton/launchers" and set the Launch Options for the shortcut to "/home/user/.local/share/native2proton/$steam_app_id/$runner_name.sh

# Known limitations

Not every game will work due to DRM and anti-cheat methods they might employ.  Some games might also require additional libraries like corefonts or vcruntimes.  These can usually be installed with Native2Proton's builtin winetricks option.  
