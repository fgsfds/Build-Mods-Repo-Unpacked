<><><><><><><><><><><><><><><><><><><><>
<><><><><><><><><><><><><><><><><><><><>

DEATH WISH ADD ON FOR BLOOD v1.6
*** README ***
by Bloatoid (bloatoid@gmail.com)

<><><><><><><><><><><><><><><><><><><><>
<><><><><><><><><><><><><><><><><><><><>


Contents:

I......... Version History, Special Thanks
II........ Installation & Ports
III....... Cut Scenes
IV........ Blood from DOSBox and Good Old Games (GOG.com) & Control / Audio Setup
V......... Play Death Wish!
VI........ The Bug Report / FAQ

***************************************
***************************************
***************************************

Part I. Version History, Special Thanks

***************************************
***************************************
***************************************

After watching a variety of Lets Play videos on Twitch and Youtube over the last few years, I’ve been slowly making edits here and there to improve Death Wish in every way possible for version version 1.6. Special thanks to the following streamers for creating especially helpful playthroughs:

Twitch:

Cubeface
Ex_mortis
GusButts
Jerryandershon
JerseyCobra
LuciferSam
MarkieMusic
Saint_Guy1
Seriouscacodemon
ShadbaseMurderTV
Ultranova5000

Youtube:

Ceekur
DemonSlay3r
Emmanuel EXE
Flairphantem
Hippo Cat
Lingyan203
LST Let's Plays
Matias FPS
Michal Fraczkiewicz
Oscar Memo
Oszkár
Pagb666
Renato Acevedo
Weavaloid

Also, special thanks to anyone else who gave Death Wish a write-up, wrote a review, mentioned it on social media, or recorded a video like Gggmanlives, JBlade, Dominic Tarason, etc. — it really helped get the word out!

The following were a big help for playtesting and fixes made to v1.5:

Elfor
fgsfds
Manhs
Nachuro
NESfag
Nyyss0nen
SkillFur

Initial conversion for v1.6 movie files to .ovg: Joseph Turano.
Nex found a bunch of v1.6 texture errors that I fixed. ( '-')-b
Pagb666 found some v1.6 secret counter issues that I fixed. d-('-' )


UPDATES

v1.6

• edits and additions to many levels across the whole campaign
• added E2M12 (secret level)
• edits to accommodate Blood: Fresh Supply users (like movie conversion to .ovg, jumping sequence adjustments, etc.)

v1.5

• large enemy spam reduction
• fixed/altered textures across many levels
• Co-Op checkpoint system
  - Teleporters close to the start of each mission will open up as players progress
  - Messages pertaining to the checkpoints only display in Co-Op mode
  - There are several missions that do not have checkpoints because they are unnecessary
  - Larger levels have depots that include multiple teleporters
  - Some basic weapons are included near teleporters so players will not need to scavenge before using them
  - Required keys are included near some teleporters so players will not always need to relocate them after respawning
• Made a bunch of fixes for Co-Op play including:
  - respawned keys/items don’t trigger events more than once
  - player placement adjustments
• Added Bloodbath levels
• Added new areas or altered architecture to every map (where the wall/sector max permitted)

v1.4

This is most of it:

Removed error in GOG config file.

Across all missions:

• Health rebalance: Last version was a little too stingy on health so I fixed that. Extra Crispy is still there for experts (including devious prox mine placement)
• Added new areas or altered architecture to every map (where the wall/sector max permitted)
• Removed some invisible walls and altered a few other things to make levels more speedrun friendly
• More multiplayer friendly
• More secrets and access to new levels
• Most switches’ height adjusted so less mouselook needed for those who use keyboard only
• More End Switches so it’s more clear that the level will end in several places
• More secrets and secret areas
• 2 new secret levels, 2 new transition levels
• Most teleporters can’t be used by enemies
• added Red Potions, Feather Fall, and Asbestos Armor to several missions

v1.3

Fixed some problems people came across during streaming play.

v1.2

Cutscene paths changed from C:\blood\ to C:\ in DW.ini
Some mission music rearranged
Enemy/respawn alterations throughout entire map set
Large reduction of Acolytes in favor of other enemy types
Some altered respawn arrangement
Miscellaneous textures aligned and altered
Many areas now favor enemy difficulty over increased numbers
Bugs and "traps" in co-op fixed

v1.1 

Actor error from e1m3 that some people are having resolved 
False keydrop in e2m3 fixed in single-player mode
e2m7 door toggle fixed for lower difficulty settings

v1.0 Original Release


***************************************
***************************************
***************************************

Part II. Installation & Ports

***************************************
***************************************
***************************************


Death Wish installs quickly and easily!

Now that you've unzipped the archive, take all the contents and drop them directly into your Blood directory. All the files have a "dw" prefix, making them group together in your folder for easy organization and searching. Nothing in Death Wish will overwrite files in your current Blood directory, and will not alter the original game in any way. 

Death Wish uses only the resources found in Blood (One Unit Whole Blood), which consists of the original game and the Plasma Pak. Cryptic Passage tiles and sounds are not used.

If you’re updating from another version, replace any files in conflict with the new ones.
 
If you're using NBlood, you have to follow the steps above, then pick dw.ini from the launch window when you start nblood.exe.

If you're using Blood: Fresh Supply, put all the DW contents in their own folder, and place that in the folder: Blood > addons. When you start FS, go to Options > Manage Addons > Death Wish

=======================================
Blood Ports
=======================================

BuildGDX
http://m210.duke4.net/

NBlood
https://nukeykt.retrohost.net/

Blood: Fresh Supply
Steam - https://store.steampowered.com/app/1010750/Blood_Fresh_Supply/
GOG.com - https://www.gog.com/game/blood_fresh_supply
Atari - https://www.atari.com/games/blood-fresh-supply/
Humble Store - https://www.humblebundle.com/store/blood-fresh-supply


***************************************
***************************************
***************************************

Part III. Cut Scenes

***************************************
***************************************
***************************************


These were replaced by new cutscenes for v1.4.

If you’re not seeing them at the beginning and end of each episode, here are the file names:

dw1a.smk
dw1a.wav
dw1b.smk
dw1b.wav
dw2a.smk
dw2a.wav
dw2b.smk
dw2b.wav
dw3a.smk
dw3a.wav
dw3b.smk
dw3b.wav

They need to be in the same directory as dw.ini when you play.

If you're using Blood:FS, they will be .ovg files:

dw1a.ovg
dw1b.ovg
dw2a.ovg
dw3b.ovg
dw3a.ovg
dw3b.ovg

***************************************
***************************************
***************************************

Part IV. Blood from DOSBox, Good Old Games (GOG.com) & Control / Audio Setup

***************************************
***************************************
***************************************

=======================================
v1.4 UPDATE #1: bMouse Replacement (I haven’t tested this so use at your own risk!)
=======================================

There’s a mouselook patch for DOS Blood that replaces bMouse. It patches blood.exe so you don't have to set up a fake external controller and launch Blood through bMouse. Compatible with Duke3D, Redneck Rampage, and Shadow Warrior. Y

http://ctpax-cheater.losthost.org/htmldocs/files/buildmfx.zip

Usage: buildmfx.exe blood.exe
And then you just set your input to "keyboard + mouse" as normal and you're good to go.

=======================================
v1.4 UPDATE #2: Someone from the /vr/ boards got GOG DW working with this. Ignore this if you're using GOG's Fresh Supply version:
=======================================

1. Extract the contents to your One Unit Whole Blood GOG folder.

2. Right click the Death Wish shortcut, click on properties and fix the 'Target' and 'Start in' location to where your gog One Unit Whole Blood folder is is. For me, as an example, this is as so:

• Start in: "C:\GOG Games\One Unit Whole Blood\"

• Target: "C:\GOG Games\One Unit Whole Blood\DOSBOX\DOSBox.exe" -conf dosboxBloodDW.conf -noconsole -c "exit"

That weird stuff 'DOSBOX.exe" -conf etc' will already be there of course. Just adjust the beginning part to make it where your target OUWB folder is.

3. Open up the dosboxBloodDW conf file in MSWord and change the IRQ value to the same as it is in your setup.exe (you could also see this value in your dosboxBlood conf file). For me, this value is '7'. Save it.

4. Get bMouse from the downloads section here:

http://swisscm.duke4.net/

Extract the files and put it in your One Unit Whole Blood directory. Note that isn't actually how you install bMouse. There's another step to do that which you'll have to read in the downloaded readme file if you want to do it but I personally don't use bMouse. It's really strange, but just having bMouse in the One Unit Whole Blood directory makes Death Wish run for me. If the file isn't in the directory, it won't work. I've experimented with this and that's just the way it is.

5. Click the DW GOG shortcut and enjoy.


=======================================
OLD HELP INFO FROM V1.3
=======================================

Installing and running Death Wish using the Good Old Games version of One Unit Whole Blood
* by Lead QA Chris Hoopes (choopes@gmail.com) *

NOTE: The default installtion directory for the GOG version of Blood on 64 bit Windows 7 is "C:\Program Files (x86)\GOG.com\One Unit Whole Blood"
We will be using that as a reference from here on out but if your intall lies somewhere else please remember to update all paths mentioned to your own.

1) All files from inside of the Death Wish zipped folder into the root Blood folder. This means that all files go into "C:\Program Files (x86)\GOG.com\One Unit Whole Blood" or whatever your root directory, NOT "C:\Program Files (x86)\GOG.com\One Unit Whole Blood\Death Wish". If your files aren't in the root directory then it won't work. Don't worry, nothing will be overwritten.

2) To enable cutscenes for the mod you may have to edit the dw.ini file to reflect your install location. Refer to Blood.ini for the correct file path if the movies work properly for the original game.

3) If you've never launched this install of Blood before you'll have to run setup.exe. You'll find a link to Setup in the shortcuts for Good Old Games One Unit Whole Blood in your Start menu. Once you're into setup (the old, ugly, weird looking blue screen) you'll need to do the following:

	1) Click Choose Sound FX Card and pick Sound Blaster
	2) Now set the following variables:
	 Address: 220
	 Sound Card Type: Sound Blaster or Compatible
	 Interrupt: 5
	 8-bit DMA: 1
	 16-bit DMA: 5
	 NOTE: if you get an error later about the interrupt, change it to 7 or another number until it works
	3) Now click Use These Settings and Continue
	 32 voices
	 16 bit mixing
	 Stereo Sound
	 44 khz
	4) Now Choose Music Card > Sound Blaster

Now that you've properly set up sound and music for a modern system you can click the test button for each. You should hear screams for the sound test and the Blood theme song for the music test.

While you're in Setup you'll also want to configure you're controls. You can rebind keyboard options within the game itself but mouse control must be set within Setup. For a more modern control scheme click Setup Mouse and then make sure that Left Button is set to Weapon_Fire and Right Button is set to Weapon_Special_Fire.

You'll also want to set up your keyboard bindings. The default controls are using the arrow keys to move, control to shoot, space to open doors, etc. You can change them either here in Setup or in-game to the more modern WASD movement scheme.

Now press Escape a few times to exit out of the Setup program and make sure to say YES to Save Setting Before Exiting.


5) Now you're ready to play! In the Blood directory where you installed the Death Wish files you should see a dosboxBloodDW.conf file. This is the DOSBox configuration file that we'll use when running Death With. These options allow for smooth fullscreen gaming and a few other nice things.

To launch the game using all of these options click the shortcut in your Blood folder called Death Wish GOG. If you look at the properties of this shortcut you'll notice that the target is set to:

"C:\Program Files (x86)\GOG.com\One Unit Whole Blood\DOSBOX\dosbox.exe" -conf dosboxBloodDW.conf -noconsole -c "exit"

If your One Unit Whole Blood install is somewhere other than the path above you'll need to edit the Target and Start In properties of that shortcut accordingly.

MOUSELOOK:

Enable by hitting the U key.

bMouse is here:

http://swisscm.duke4.net/
As of 11/1/11 the latest version is swisscm.duke4.net/downloads/bMouse06.ZIP with a GOG.com discussion at:
http://www.gog.com/en/forum/blood_series/bMouse_0_5_mouse_driver_that_fixes_the_terrible_mouselook_on_dos_build_games/page1

To get bMouse working, copy bMouse.exe into your Blood directory.

Now edit your BLOOD.CFG and change the following values:
quote:

 ExternalFilename = "bMouse.EXE" (this tells the game to use bMouse as an "external device" executable)
 MouseAiming = 0
 MouseAimingFlipped = 0
 ControllerType = 3 (sets the game to use Keyboard and External, in other words, Keyboard and External application bMouse.exe to "control" the mouse)
 MouseAnalogScale1 = -65536 (if you do not do this, your mouse will be inverted)
 MouseAim = 1 (turns on mouse aim, obviously)


The end of your dosboxBloodDW.conf file should look like this:
quote:

[autoexec]
# Lines in this section will be run at startup.

@ECHO OFF
mount C "."
imgmount D game.inst -t iso
c:
cls
BMOUSE.EXE LAUNCH BLOOD.EXE -ini dw.ini
dw
exit

The BMOUSE.exe line being the important one. You won’t need this if you’re using buildmfx (see Part IV, update #2).


And this might be optional but I noticed that the Good Old Games install contains an outdated version of DOSBox. I updated to .74 by overwriting these files in the DOSBox folder:
quote:

 dosbox.exe
 SDL.dll
 SDL_net.dll
 zmbv/zmbv.dll
 zmbv/zmbv.inf


Of course make backups of anything you overwrite first but this version of DOSBox is supposed to play better with Blood. Hope this all works because it seems to run fine for me! 


***************************************
***************************************
***************************************

Part V. Play Death Wish!

***************************************
***************************************
***************************************


The file dw.bat will fire up Death Wish! It follows this command:

blood -ini dw.ini

This can be edited to suit your needs, just as the dw.ini file can. You'll want to play Death Wish through the .ini file to get the full experience (rather than playing them one-by-one in DOS), which includes music, on-screen messages, difficulty settings, cut scenes, etc.

If you are using DOSBox or a similar program, just navigate to your blood directory and type dw


***************************************
***************************************
***************************************

Part VI. The Bug Report / FAQ

***************************************
***************************************
***************************************


Q: The cutscenes don't appear / have sound. How do I fix it?
A: See Part III. The movies (.smk) and sound (.wav) need to be in the same directory as dw.ini. For Blood:FS, the .ovg files need to be there as well.

Q: A cutscene is running really slowly. What’s wrong?
A: This is a port/DOSBox error, not an error with the DW files. Occasionally when this happens it works fine the next time it loads. I’m not sure what causes this error. 

Q: When I try and run DW.bat with DOSBox I get an error message saying "src\sound.cpp(516): Playback failed, possibly due to an invalid or conflicting IRQ" 
A: Go through Part IV to make sure your sound is configured correctly. Even if you aren't running the GOG version the sound setup is still applicable. If you're sound if configured properly, this may happen once in a blue moon anyway, in which case restarting DOSBox should fix the problem.

Q: I keep getting ERROR src\actor.cpp
A: This comes from the 2 "pod" enemies from Plasma Pak. They are buggy and will sometimes crash the game when they try to fire at the player. Blame whoever programmed these things into the game. They would always crash a game if they fired their projectiles over a linked sector or water, too, so I had to make sure not to put them anywhere near those effects. 

Q: I'm playing Lost Highway/Spooky World/Mothership/The Room and this moving sector is totally glitched up.
A: This is an engine error that occurs with path sectors sometimes and can be fixed by restarting the level. In Lost Highway, where I first wanted to use this effect, I tried a sliding sector that moved back and forth forever, and that broke the game WAY more.

Q: My mouse isn't working properly.
A: See Part III for controller configuration.

Q: There's no music in E1M1 (Home Sweet Home) when I start a new game.
A: This occurs sometimes on the Mac version of DOSBox. If you level skip to the second mission (type "mario 1 2") then restart your game the music should work normally.

Q: The darkness/depth-fog is gone when I load my game.
A: Start a new game up on E1M1, THEN load your saved game. If you boot up Blood and go directly to your saved game it will sometimes cause the lighting error.

Q: I was walking between 2 trees / into an acute corner / a tight space and died.
A: This is a Blood engine bug, where even if the sector is not marked as "crushing" it will kill you anyway.

Q: I was on the moving Pod in Mothership and fell to my doom.
A: It's a complex path sector, so it's best if you aren't moving around too much. It has a bunch of blocking sectors to prevent this but someone who is jumping and running around can trigger the glitch anyway.

Q: The [insert enemy here] is acting strangely.
A: I didn't program any of the enemy behaviors. Sometimes that act strangely when moving on top of sprites or can get stuck when they walk into a corner. I also have nothing to do with that glitch where enemies stay lit on fire but don’t die! Just hit them with a flare/explosive/spraycan/life leech — hitscan weapons won’t work.

Q: [insert problem here] happens when I use [anything other than DOSBox to play].
A: I only used the vanilla assets for Blood — I didn’t add anything. If you see a problem when you play using a port, contact the port developers. 

