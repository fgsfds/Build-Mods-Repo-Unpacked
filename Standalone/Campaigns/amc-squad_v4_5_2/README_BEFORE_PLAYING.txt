
======= WELCOME TO THE AMC SQUAD! ==========

Thank you for downloading our game!

This document provides some first time instructions on how to properly install the game, how to play, configure your settings, and other useful information.

--- Table of Contents ---

1. General Information
2. Install Instructions
  2.1 Windows Instructions
  2.2 Linux Instructions
3. System Requirements
4. Custom Settings
5. Streaming / Recording Video
6. Level Editor
7. Known Issues
8. Final Notes

======= GENERAL INFORMATION ==========

AMC Squad isn't your typical 90s "Boomer Shooter"!

While there's plenty of fast-paced Build Engine gameplay to be found, the game also features many more advanced mechanics and an overarching story
that leads you through a variety of missions. We highly recommend taking it slow and exploring the world to get the most out of the game.

When playing AMC Squad for the first time, you should start with the first episode 'The Men who were AMC' and choose Normal difficulty.

While the basic gameplay is similar to that of classic Build Engine games, there are many additional mechanics that you should become familiar
with first before playing on a higher difficulty. Higher skill levels introduce new mechanics that you will be unprepared for, and may even be
underequipped to deal with. Note that the game is structured such that you can always increase the difficulty later on without restarting the
game in its entirety.

The game features a large roster of different characters to choose from, each with a different set of weapons and abilities. Some missions are
designed for specific characters, while others let you freely choose who you want to play as. For the first mission, we recommend choosing James,
as he provides a basic set of abilities that are easy to use and get familiarized to.

The level progression is mission-based, and the levels are typically selected through a map screen that you can navigate around in.
While the game starts out linearly, the missions later branch out, and you get to choose them in different orders, some of which are entirely optional.

The game saves your progress automatically while playing. Save files are available, but are not required to save your progress between missions.
The option "Continue at AMC Base" can be used to continue at the point in the story where you left off.

Finally, there's an option called "Game Settings" in the main menu. This contains a number of options specific to AMC that you may want to change.
A more detailed explanation is given below, in the section "Custom Settings".

Most other details should be explained while in the game itself. Have fun!

If you have any questions, feel free to ask us on IndieDB, itch.io or the AMC Discord:
* IndieDB : https://www.indiedb.com/games/the-amc-tc
* itch.io : https://amcsquad.itch.io/game
* Discord : https://discord.gg/aCqnMAZ

======= INSTALL INSTRUCTIONS ==========

--- Windows Instructions ---

1. Extract the contents of the zip into an empty folder.
  - Important: !!! DO NOT EXTRACT THE PACKAGE INTO AN EXISTING "AMC TC" OR "AMC SQUAD" FOLDER !!!
2. If you played a previous release of the game, first run the tool "progress_import.exe" to import data from your old installation folder.
3. Afterwards, or if you play for the first time, simply run "amcsquad.exe".

Note that the first startup may take longer than normal, as it needs to cache sounds and textures. Subsequent startups will be much faster.

If interested, the source for the progress import tool can be found at: https://github.com/dibollinger/amctc_dataimporter

--- Linux Instructions ---

1. Extract the contents of the zip into an empty subfolder within your home directory.
  - Important: !!! DO NOT EXTRACT THE PACKAGE INTO AN EXISTING "AMC TC" OR "AMC SQUAD" FOLDER !!!
2. Go to https://github.com/dibollinger/amcduke32/ and follow the compile instructions to build both the `amcsquad` and `mapster32` binaries.
  - Alternatively, you can also try to use one of the precompiled binaries on the releases page, but we cannot guarantee that they will work on every system: https://github.com/dibollinger/amcduke32/releases
3. Note that with every release of AMC Squad, there are significant changes to the game binaries, hence we recommend compiling a build with the appropriate release tag for a new installation.
4. Finally, copy the compiled binaries over into the base folder of your AMC Squad directory, and then launch the game.
5. If you had a previous version of the game installed in a different folder, you will need to copy the following files from your old installation directory into the new one:
  - `./DATA/*.AMCTC`
  - `./amcsquad.cfg`
  - `./settings.cfg`
6. These files contain all settings and progress of your previous installation. Simply overwrite any existing files in the new installation, and you're good to go.

Note that the first startup may take longer than normal, as the game needs to cache sounds and textures. Subsequent startups should be much faster.

======= SYSTEM REQUIREMENTS ==========

The approximate system requirements are:

    Minimum:
        Requires a 64-bit processor and operating system
        OS: Windows 7/8/8.1/10/11 or Linux (tested with Debian-based distributions)
        Processor: Intel Core i5, AMD Ryzen or equivalent
        Memory: 2048 MB RAM
        Graphics: 1024 MB video memory. Intel integrated graphics supported.
        Storage: 2 GB available disk space

    Recommended:
        Requires a 64-bit processor and operating system
        OS: Windows 10/11 or Linux (tested with Debian-based distributions)
        Processor: Intel Core i5, AMD Ryzen or equivalent
        Memory: 4096 MB RAM
        Graphics: 2048 MB or more dedicated video memory. NVIDIA or AMD preferred.
        Storage: 2 GB available disk space

Note that MacOS is currently NOT officially supported.

As of version 4.5.0 of AMC Squad, the OpenGL (Polymost) renderer is the default, and the "Software Mode" renderer can no longer be selected from the menu.

If you still need to use the old Software renderer, it can be selected through the console via the command "setrendermode 0".
Note that we will not provide any support or bugfixes for this renderer, and graphical glitches are to be expected.

======== CUSTOM SETTINGS =========

As of version 4.0.0, AMC Squad includes a custom options menu not found in other eduke32 builds.

The following options are currently available:

* Photosensitivity mode
  - Reduces the intensity of screen flashing, texture flickering and other similar effects. If any flashing effects remain with this setting active, please report them as a bug.

* Streamer Mode
  - Replaces music that may be recognized by Twitch/Youtube and other streaming services as copyrighted tracks. Also disables potentially offensive material that may get videos demonetized.

* Disable Facehugger Enemies
  - Disables any enemies that may attach to the screen, such as the classic face-eating slime monsters. Please report if any facehugger enemies still appear after enabling.

* Disable Quick Time Events
  - Disables all dynamic interactions where the attack button or similar needs to be mashed. Does not include certain scripted sequences.

* Disable spiders
  - Replaces and removes all enemies that are or look like spiders. Please create a bug report if any spiders still appear with the setting active.

* Vanilla Item Selection
  - Replaces the item wheel with the classic left/right item selection.

* High Visibility Items
  - Items are highlighted and are made more visible when this option is active.

* Centered Prompt Position
  - When disabled, interact icons will appear closer to the center of the screen, near the crosshair. When enabled, they will be placed centered at the bottom of the screen instead.

* Randomize Enemies in Usermaps
  - Randomizes enemy types when loading a custom map in the main menu. This does not include any maps loaded through the mission select screen.

* Dynamic Music in Usermaps
  - Play dynamic music when loading a custom map in the main menu. This does not include any maps loaded through the mission select screen.

* Show Helmet Overlay in HUD
  - Certain characters have a helmet overlay active while playing. When this is set to "no", these overlays will no longer appear.

* Boss Healthbars
  - Change the look and style of the health bar that appears when fighting a boss.
  - Off: No health bar
  - Basic: Basic health bar style
  - Basic + Name: Basic health bar style, with the boss name shown below.
  - Fancy: Health bar that matches the faction of the boss being fought.
  - Fancy + Name: Fancy health bar style, with the boss name shown below.

* Change Slow-motion frequency
  - When killing enemies, a slow-motion effect may randomly occur. This options allows changing the frequency of this effect, or disabling it entirely.

* HUD Glass Effects
  - For some characters, there are on-screen effects that simulate effects of glass of a helmet or visor. Disable this setting to deactivate these effects.

* Enable Subtitles
  - Enables subtitles during cutscenes and during in-game dialogue.

* Show Speech Bubbles
  - If enabled, speech bubbles will be shown over NPCs that can be interacted with.

* Big UI Cursor
  - If enabled, the cursor for in-game UIs will be twice as large. Does not affect the cursor on the main menu.

* Bright UI Cursor
  - If enabled, the cursor for in-game UIs will appear in a bright yellow color, to make it more visible. Does not affect the cursor on the main menu.

* Enemy Protection Sound
  - Some enemies are resistant or immune to certain damage types. If enabled, a sound is played if your attacks are less, or even ineffective.

* Character Voice Delay
  - Changes the delay for one-liners in-game. To disable them complete, enable the "Silent Protagonist" mode in the "Sound Setup".

* Dynamic Weapon Glow
  - If enabled, will display dynamic glow effects on weapons. May improve performance if disabled.

* Gold Sparkle Effects
  - If enabled, will display a gold sparkle effect on golden weapons. May improve performance if disabled

* Disable Rain/Snow Effects
  - If set to "yes", rain and snow will be disabled on levels that normally have these effects.

* Glass Shards
  - When breaking certain objects, glass shards are normally spawned that linger on. If disabled, these shards will disappear immediately.

* Advanced Flame Effects
  - If enabled, the game will display fancy flame effects in certain locations, such as torches. May improve performance if disabled.

* Highres Clouds
  - Controls the quality of certain cloud actors. May improve performance if reduced or disabled.

* Particle Effect Distance
  - Changes the distance at which particles like flames or rain are spawned. Improves performance if he distance is reduced.

======== STREAMING / RECORDING VIDEO =========

Streamer mode is an option available inside the settings menu. Rather than needing to manually replace music, you can now toggle this option to prevent accidental copyright claims or demonetization.

While most of the music in the mod is custom-made or under free licenses, there are some tracks that may still trigger the automatic detection systems.
This setting will replace the known problematic tracks with safe alternatives.

This setting will also disable certain textures and sprites that may be considered offensive or not safe for streaming/recording video.

Please report if any of your videos or streams of AMC Squad encounter copyright issues, we will try to address the problem and add the offending material under this option.

======== LEVEL EDITOR ========

If you are interested in creating levels or mods for the game, use the packaged "mapster32.exe" binary.

This is the same level editor as used with games such as Duke Nukem 3D. If you are just starting out, we recommend first learning the basics of level editing of Duke 3D, as the process for AMC is similar:
* https://infosuite.duke4.net/

Here is an assortment of different resources to help you get started, in no particular order:
* https://www.youtube.com/watch?v=kfNGj1jB1Tc
* https://wiki.eduke32.com/wiki/Build/Mapster32_Keyboard_Commands
* https://www.youtube.com/watch?v=mnN-2fCcweo
* https://www.youtube.com/watch?v=pAwM8eSRHtQ
* https://docs.google.com/document/d/14yVNQRxyZpiA3nIqQbiPRsLR2vUwyu2810XZF8UR0bU/edit
* https://docs.google.com/document/d/1vII1ILXvNjCYhdo-As7ndoKUbeXnHW8elS4ieZWWWTw/edit

Note that you should always use the version of mapster32 packaged with AMC Squad to create maps for AMC.

Other mapster32 builds may not work properly and could corrupt your AMC Squad maps if saved with them.


====== KNOWN ISSUES ==========

* There is a large startup delay related to voxel and sound preloading. The game may take between 15 to 30 seconds to fully initialize on first boot.

====== FINAL NOTES ===========

As of Version 3.6 and up, AMC TC/AMC Squad uses a fork of eduke32 called "amcduke32", which changes certain engine behavior and adds additional features that are required by the game.

The source can be found here: https://github.com/dibollinger/amcduke32

Note that AMC Squad will not work with regular eduke32 builds!

Many thanks to the eduke32 team, without whom this fork would not exist.

EDuke32 and Build are licensed under GPL 2.0 and the BUILD license, which we have included in this download.
