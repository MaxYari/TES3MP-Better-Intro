# Better new character intro/beginning for [TES3MP](https://tes3mp.com/) version 0.7.x.

**Based on** [StartupScript](https://github.com/Skvysh/TES3MP-Scripts/tree/master/StartupScripts) with few minor tweaks.

This scripts bring new character experience closer to the single-player Morrowind. 
Instead of being spawned on the streets of Balmora, new characters appear on the imperial ship and go through census office as usual albeit without character generation process in the office.

## Installation
Drag'n'Drop solution for lazy, paste contents of this archive into OpenMW/mp-stuff replacing the original files. 
If cells affected by this script were already intialised - they should be removed (by removing files with corresponding cell names in `mp-stuff/data/cell`), be warned that removing those files would reset all of the changed done to those cells by players.
If you don't care and/or this is a fresh server - just remove everything in that folder.
If you've already altered script/config files present in this repo and don't want to replace them - you'd better follow instructions (linked above) on installing StartupScripts and enabling census and excise office.

## Issues
If you keep `config.shareJournal = true` in `config.lua` - only one player can go through the door near the final intro guard after asking about duties. Others will be prompted by the door to ask about duties. To unstuck this - the very first door (from the ship to the office) is not locked - so you can go back to the pier and around the office.