<><><><><><><><><><><><><><><><><><><><>
<><><><><><><><><><><><><><><><><><><><>

DEATH WISH ADD ON FOR BLOOD v1.3
*** README ***
by Bloatoid (bloatoid@gmail.com)

<><><><><><><><><><><><><><><><><><><><>
<><><><><><><><><><><><><><><><><><><><>


Contents:

I......... Version History
II........ Installation
III....... Making the Cut Scenes Work
IV........ Blood from Good Old Games (GOG.com) & Control / Audio Setup
V......... Play Death Wish!
VI........ The Bug Report / FAQ

***************************************

Part I. Version History

***************************************

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
README expanded to include info on running Death Wish on the GOG.com version of Blood
README expanded to include info on bMouse for mouselook

v1.0 Original Release


***************************************

Part II. Installation

***************************************

Death Wish installs quickly and easily!

Now that you've unzipped the archive, take all the contents and drop them directly into your Blood directory. All the files have a "dw" prefix, making them group together in your folder for easy organization and searching. Nothing in Death Wish will overwrite files in your current Blood directory, and will not alter the original game in any way. 

Death Wish uses only the resources found in Blood (One Unit Whole Blood), which consists of the original game and the Plasma Pak. Cryptic Passage tiles and sounds are not used.


***************************************

Part III. Making the Cut Scenes Work

***************************************

A little movie should play at the beginning and end of each episode in Death Wish. They will only play if the dw.ini file trees are set up correctly, though.

If you open dw.ini you will see a section in the beginning of each episode that looks like this:

[Episode1]
CutSceneA=C:\dw1a.smk
CutWavA=C:\dw1a.wav
CutSceneB=C:\dw1b.smk
CutWavB=C:\dw1b.wav


These reference the movies (.smk) and soundtracks for them (.wav). As you can see, the default setup assumes you have set up your Blood directory as C:\Blood. If this is the case, you don't have to edit anything. If your Blood directory exists elsewhere, you will have to edit the dw.ini file and save it. If you have your directory in C:\Games\Blood for example, you will have to change your dw.ini to read:

[Episode1]
CutSceneA=C:\Games\Blood\dw1a.smk
CutWavA=C:\Games\Blood\dw1a.wav
CutSceneB=C:\Games\Blood\dw1b.smk
CutWavB=C:\Games\Blood\dw1b.wav

Remember, you will have to repeat this task for all 3 episodes! 

If you have your copy of Blood from Good Old Games (GOG.com), you may need to do some other things:

Do your movies for regular Blood work properly? If so, that may be good news!
Death Wish's ini file is basically a mirror of the original game's. So, if you dropped all the contents directly into the Blood folder, you should be able to open Blood.ini and see what file paths it is using to access its movies (cs1.smk, etc) and use that in Death Wish's ini.

One player cited:
"The blood.ini literally only read as "CutSceneA=cs1.smk" as opposed to having a file path toward cs1.smk.
So I opened dw.ini , removed the file paths so that it only read "CutSceneA=dw1a.smk" and Hey-Presto! Lovely DeathWish Intro."

I've had some people say the audio does not play with this method for some reason, and will only work after adding the C:\ in front. Audio should play with each movie.

If this doesn't work, move on to Part III for a more detailed rundown by Chris.


***************************************

Part IV. Blood from Good Old Games (GOG.com) & Control / Audio Setup

***************************************

Installing and running Death Wish using the Good Old Games version of One Unit Whole Blood
* by Lead QA Chris Hoopes (choopes@gmail.com) *

NOTE: The default installtion directory for the GOG version of Blood on 64 bit Windows 7 is "C:\Program Files (x86)\GOG.com\One Unit Whole Blood"
We will be using that as a reference from here on out but if your intall lies somewhere else please remember to update all paths mentioned to your own.

1) All files from inside of the Death Wish zipped folder into the root Blood folder.  This means that all files go into "C:\Program Files (x86)\GOG.com\One Unit Whole Blood" or whatever your root directory, NOT "C:\Program Files (x86)\GOG.com\One Unit Whole Blood\Death Wish".  If your files aren't in the root directory then it won't work.  Don't worry, nothing will be overwritten.

2) To enable cutscenes for the mod you may have to edit the dw.ini file to reflect your install location. Refer to Blood.ini for the correct file path if the movies work properly for the original game.

3) If you've never launched this install of Blood before you'll have to run setup.exe.  You'll find a link to Setup in the shortcuts for Good Old Games One Unit Whole Blood in your Start menu.  Once you're into setup (the old, ugly, weird looking blue screen) you'll need to do the following:

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

Now that you've properly set up sound and music for a modern system you can click the test button for each.  You should hear screams for the sound test and the Blood theme song for the music test.

While you're in Setup you'll also want to configure you're controls. You can rebind keyboard options within the game itself but mouse control must be set within Setup.  For a more modern control scheme click Setup Mouse and then make sure that Left Button is set to Weapon_Fire and Right Button is set to Weapon_Special_Fire.  This is of course entire preferencial but it's important to know where you can change this functionality.

You'll also want to set up your keyboard bindings as well.  The default controls are using the arrow keys to move, control to shoot, space to open doors, etc.  You'll need to change them either here in Setup or in-game to the more modern WASD movement scheme.

Now press Escape a few times to exit out of the Setup program and make sure to say YES to Save Setting Before Exiting.


5) Now you're ready to play!  In the Blood directory where you installed the Death Wish files you should see a dosboxBloodDW.conf file.  This is the DOSBox configuration file that we'll use when running Death With.  These options allow for smooth fullscreen gaming and a few other nice things.

To launch the game using all of these options click the shortcut in your Blood folder called Death Wish GOG.  If you look at the properties of this shortcut you'll notice that the target is set to:

"C:\Program Files (x86)\GOG.com\One Unit Whole Blood\DOSBOX\dosbox.exe" -conf dosboxBloodDW.conf -noconsole -c "exit"

If your One Unit Whole Blood install is somewhere other than the path above you'll need to edit the Target and Start In properties of that shortcut accordingly.

MOUSELOOK:

Enable by hitting the U key.

For "true" Mouselook, you'll need bMouse from the downloads section of http://swisscm.duke4.net/
As of 11/1/11 the latest version is swisscm.duke4.net/downloads/BMOUSE06.ZIP with a GOG.com discussion at:
http://www.gog.com/en/forum/blood_series/bmouse_0_5_mouse_driver_that_fixes_the_terrible_mouselook_on_dos_build_games/page1

From Chris:

OK so I got bMouse working. Turns out the only reason it didn't before is that I fucked up and put it in the wrong Blood install because I have so many of them.


So to get bMouse working, copy bmouse.exe into your Blood directory.

Now edit your BLOOD.CFG and change the following values:
quote:

    ExternalFilename = "BMOUSE.EXE" (this tells the game to use bmouse as an "external device" executable)
    MouseAiming = 0
    MouseAimingFlipped = 0
    ControllerType = 3 (sets the game to use Keyboard and External, in other words, Keyboard and External application bmouse.exe to "control" the mouse)
    MouseAnalogScale1 = -65536 (if you do not do this, your mouse will be inverted)
    MouseAim = 1 (turns on mouse aim, obviously)


Now at the end of your dosboxBloodDW.conf file edit the end so it looks like this:
quote:

    [autoexec]
    # Lines in this section will be run at startup.

    @ECHO OFF
    mount C "."
    imgmount D game.inst -t iso
    c:
    cls
    BMOUSE.EXE LAUNCH BLOOD.EXE -ini dw.ini
    #dw
    exit


The bmouse.exe line being the important one.


And this might be optional but I noticed that the Good Old Games install contains an outdated version of DOSBox. I updated to .74 by overwriting these files in the DOSBox folder:
quote:

    dosbox.exe
    SDL.dll
    SDL_net.dll
    zmbv/zmbv.dll
    zmbv/zmbv.inf


Of course make backups of anything you overwrite first but this version of DOSBox is supposed to play better with Blood. Hope this all works because it seems to run fine for me! 


***************************************

Part V. Play Death Wish!

***************************************

The file dw.bat will fire up Death Wish! It follows this command:

blood -ini dw.ini

This can be edited to suit your needs, just as the dw.ini file can. You'll want to play Death Wish through the .ini file to get the full experience (rather than playing them one-by-one in DOS), which includes music, on-screen messages, difficulty settings, cut scenes, etc.

If you are using DOSBox or a similar program, just navigate to your blood directory and type dw



***************************************

Part VI. The Bug Report / FAQ

***************************************


Q: The cutscenes don't work!
A: See Part II & III of this README.

Q: When I try and run DW.bat with DOSBox I get an error message saying "src\sound.cpp(516): Playback failed, possibly due to an invalid or conflicting IRQ" 
A: Go through Part III to make sure your sound is configured correctly. Even if you aren't running the GOG version the sound setup is still applicable. If you're sound if configured properly, this may happen once in a blue moon anyway, in which case restarting DOSBox should fix the problem.

Q: I keep getting ERROR src\actor.cpp
A: This comes from the 2 "pod" enemies from Plasma Pak. They are buggy and will sometimes crash the game when they try to fire at the player. Blame whoever programmed these things into the game. I like the pod enemies but I almost regret deciding to use them since they are so unstable. They would always crash a game if they fired their projectiles over a linked sector or water, too, so I had to make sure not to put them anywhere near those effects. What a pain.

Q: I'm playing Lost Highway/Spooky World/Mothership/The Room and this moving sector is totally glitched up.
A: This is an engine error that occurs with path sectors sometimes and can be fixed by restarting the level. Save often, kids! In Lost Highway, where I first wanted to use this effect, I tried a sliding sector that moved back and forth forever, and that broke the game WAY more.

Q: My mouse isn't working properly.
A: See Part III for controller configuration.

Q: There's no music in E1M1 (Home Sweet Home) when I start a new game.
A: This occurs sometimes on the Mac version of DOSBox. If you level skip to the second mission (type "mario 1 2") then restart your game the music should work normally.

Q: I was walking between 2 trees / into an acute corner / a tight space and died.
A: This is a Blood engine bug, where even if the sector is not marked as "crushing" it will kill you anyway. Just be careful.

Q: I was on the moving Pod in Mothership and fell to my doom.
A: It's a complex path sector, so it's best if you aren't moving around too much. It has a bunch of blocking sectors to prevent this but someone who is jumping and running around can trigger the glitch anyway.

Q: The [insert enemy here] is acting strangely.
A: I didn't program any of the enemy behaviors. Sometimes that act strangely when moving on top of sprites or can get stuck when they walk into a corner. 

