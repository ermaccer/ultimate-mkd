<p align="center"><img src=https://i.imgur.com/Hjf4Gsg.png></p>

<p align="center">New characters, stages and more!</p>


# Intro

Ultimate Mortal Kombat Deception is a modification for PS2 version of Mortal Kombat Deception. A custom PCSX2 fork provides easier way to edit code and also more available RAM.

### NOTE: Current PS2 support is experimental, if it works it works - unless you find a crash that's easily reproducible I'm afraid there's nothing that can be done!


# Features

## New Characters

| Name | Status | Video |
|       ---       |       ---       |      ---       |
| Sonya | ✅ Done | https://youtu.be/ODtz7OYI5SE |
| Kitana | ✅ Done | https://youtu.be/gED1Q2LSpAo |
| Jax | ✅ Done | https://youtu.be/5wcyICiY3FM |
| Frost | ✅ Done| https://youtu.be/JAA1lc9ZeXE |
| Blaze | ✅ Done| https://youtu.be/ZvAlTYgY8xo |
| Shao Kahn | ✅ Done | https://youtu.be/voCa6wB3bRE |
| Goro | ✅ Done | https://youtu.be/pJpnEWbMQds |
| Drahmin | ✅ Done| https://youtu.be/jKyuNLhHfoo |
| Sareena | ✅ Done | https://youtu.be/M7JsnM7SLM0 |
| Quan Chi | ✅ Done | https://youtu.be/oC72se-mPO8 |



# Download
Current version: **V4**

Check for files https://github.com/ermaccer/ultimate-mkd/releases

Video How To Install: https://www.youtube.com/watch?v=HAX8KxVIRt0


### All new characters can be accessed by pressing L3 as any player on the select screen!



# Screenshots
![](https://raw.githubusercontent.com/ermaccer/ultimate-mkd/master/img/1.jpg)
![](https://raw.githubusercontent.com/ermaccer/ultimate-mkd/master/img/2.jpg)
![](https://raw.githubusercontent.com/ermaccer/ultimate-mkd/master/img/3.jpg)
![](https://raw.githubusercontent.com/ermaccer/ultimate-mkd/master/img/4.jpg)
![](https://raw.githubusercontent.com/ermaccer/ultimate-mkd/master/img/5.jpg)
![](https://raw.githubusercontent.com/ermaccer/ultimate-mkd/master/img/6.jpg)
![](https://raw.githubusercontent.com/ermaccer/ultimate-mkd/master/img/7.jpg)

## Changelog

**V4**
 - New characters: Drahmin, Sareena and Quan Chi
 - Locked death traps for Blaze on Sky Temple, Lower Mines and Dark Prison due to issues
 - Frost now plays female sounds correctly when getting up
 - Frost's throw now does 2 damage sections instead of 3
 - Kitana's D3 in Eagle Claw no longer crashes the game
 - Fixed corrupted slot in alternate select screen
 - Fixed glitched kontent item names
 - Ladder models are now loaded from `kon_unique_npcs.ssf`

**V3**
 - New character: Goro
 - New lifebar and select screen icons for Sonya
 - General Frost stability updates
 - NPC select has been removed from the default settings, its possible to reenable it in the .ini settings file
 - Added full chess kombat support for new characters with the exception of Onaga
 - New characters and stages will now properly appear on the arcade ladder  
 - Hold L1 and SQUARE in Gameplay options menu to view current UMKD version 
 - A rare crash on Kitana's winpose should be fixed
 - Fixed new textures, blending settings no longer need to be changed
 - Fixed a crash while perfoming Jax's gun on certain stages
 - Fixed Puzzle Kombat, no longer crashes the game

  
**V2**
 - Three new characters: Blaze, Frost and Shao Kahn
 - Kitana special moves sounds are now affected by sound settings
 - New fatalities no longer pause for a while after they are finished

**V1**
 - Three new characters: Jax, Kitana and Sonya
 - New restored stage: Katakombs
 - Fully randomized ladders
 - Onaga tweaks (movelist, no intro)
 - Konquest stages & dojos available in normal stage selection


# PS2 vs PC
PS2 support was added in the V3 version of UMKD, it is currently experimental and some features (nothing gameplay related) have been cut when compared to the PC (emulated) version.

## Cut features
- In-game menu (L3)
- No camera options
- No NPC select to save on bytes
- No ini configuration


## Konquest mode

Since the mod pushes PS2 executable hard enough, it is not recommended to play Konquest on the UMKD modded version of MKD.

# Repos
https://github.com/ermaccer/MKDHook - MKDHook is responsible for all code changes.

https://github.com/ASI-Factory/PCSX2-Fork-With-Plugins/releases - A fork of PCSX2 which adds plugins