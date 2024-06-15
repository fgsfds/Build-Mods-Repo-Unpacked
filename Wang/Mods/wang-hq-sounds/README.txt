====ABOUT=====

This mod replaces original sounds with high quality ones based on actual sources. If a specifc source was not found, then a sound was upscaled.

Lo Wang voice was upscaled using Voice Fixer https://huggingface.co/spaces/akhaliq/VoiceFixer

This package contains sounds sample rated to 44 kHz, encoded PCM signed 16 bit, mono, saved as Sound Blaster (VOC) format.

====HOW TO USE=====

Raze: 

	1. Drag and drop this ShadowWarriorHQSounds_VOC.zip onto Raze.exe and select Shadow Warrior as game.

	Alternatively you may set either an absolute or relative path in raze_portable.ini to ShadowWarriorHQSounds_VOC.zip located e.g. in "autoload" folder, like this:

	Absolute path:

	[ShadowWarrior.Autoload]
	Path=C:\Games\Raze\autoload\ShadowWarriorHQSounds_VOC.zip

	Relative path:

	[ShadowWarrior.Autoload]
	Path=autoload\ShadowWarriorHQSounds_VOC.zip

	2. In game go to Sound Options -> Advanced Options -> Turn on "Ignore file type for sound lookup".
	3. Close and relaunch Raze to apply that change.

BuildGDX: 

	1. Drop ShadowWarriorHQSounds_VOC.zip into your "autoload" directory.

	2. Make sure the autoload option in the launcher is checked.

VoidSW:

	1. Put ShadowWarriorHQSounds.zip in Shadow Warrior game folder (not "autoload" directory).

	2. Make a shortcut of voidsw.exe.

	3. Right click on created shortcut and select Properties.

	4. Add parameter "-gShadowWarriorHQSounds_VOC.zip" to the Target.

		Example: "C:\Games\Shadow Warrior\voidsw.exe" -gShadowWarriorHQSounds_VOC.zip
	
	5. Launch VoidSW using created shortcut of it.

====KNOWN ISSUES=====

VoidSW and BuildGDX do not load sounds from "filter" subfolder, that means custom sounds from addons will not be replaced.

This issue can be somewhat resolved by directly replacing sounds in GRP containers but after this change VoidSW might no longer detect
GRPs as the checksum changes. To run the game VoidSW has to be run with command line "-gamegrp [file.grp]". BuildGDX shouldn't have any issues with that.

The tool which can replace sounds in GRP:
https://dukeworld.com/2001-current/rtcm/duke3d-tools-grp/gfs31.zip

====CREDITS=====
Project lead:
Dzierzan

Sound hunters:
Dzierzan, Shadow (Ninjakitty), Akis_02

Sound recreation:
Dzierzan, Akis_02

Sound upscaling:
Dzierzan, epicjack340, DeevDaRabbit