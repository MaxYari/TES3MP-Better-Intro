# Better new character intro/beginning for [TES3MP](https://tes3mp.com/) version 0.7.0-alpha.
(May work on later versions as well)

**Based on** [StartupScript](https://github.com/Skvysh/TES3MP-Scripts/tree/master/StartupScripts) with few minor tweaks.

These scripts bring new character experience closer to original Morrowind. 
Instead of being spawned on the streets of Balmora - new characters appear aboard the imperial prison ship and go through the census office, albeit without character generation process in it.

## Installation
Drag'n'Drop solution for lazy, paste contents of this archive into OpenMW/mp-stuff replacing original files.
 
If cells affected by this script were already initialised - they should be removed (by removing files with corresponding cell names in `mp-stuff/data/cell`), be warned that removing those files will reset all of the changes done to those cells by players.
If you don't care and/or this is a fresh server - just remove everything in that folder.

If you've already altered script/config files that this repo is about to replace and don't want to do so - you'd better follow instructions (linked above) on installing StartupScripts and enabling census and excise office.

## Removing the ship
If you want to remove the ship, for ex if you are playing coop and already gone through the intro area and now don't want to see the prison ship anchored at Seyda Neen at all times:

In `scripts/contentFixer.lua` find `Delete the chargen boat and associated guards and objects` line and uncomment 3 lines below it (remove `--` in the beginning of each line).

On the next server startup boat and related guards will be removed.

## Issues
If you keep `config.shareJournal = true` in `config.lua` - only one player can go through the door near the final intro guard after asking about duties. Others will be prompted by the door to ask about duties. To unstuck this - the very first door (from the ship to the office) is not locked - so you can go back to the pier and around the office.