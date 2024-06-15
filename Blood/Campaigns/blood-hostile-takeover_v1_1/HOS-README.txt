<><><><><><><><><><><><><><><><><><><><>
<><><><><><><><><><><><><><><><><><><><>

HOSTILE TAKEOVER ADD ON FOR BLOOD v1.1
*** README ***
by Bloatoid (bloatoid@gmail.com)

<><><><><><><><><><><><><><><><><><><><>
<><><><><><><><><><><><><><><><><><><><>


Contents:

I......... Version History
II........ Installation
III....... Making the Cut Scenes Work
IV........ Blood from Good Old Games (GOG.com) & Control / Audio Setup
V......... Play Hostile Takeover!
VI........ The Bug Report / FAQ

***************************************

Part I. Version History

***************************************
v1.1
Added Co-Op starting points to all levels
Fixed some textures here and there
Changed some secrets around
Added more health to overall game
Ammo added to some levels
Secret Counters now work
Eliminated some backtracking segments
Some minor architectural changes to levels

v1.0 Original Release


***************************************

Part II. Installation

***************************************

Hostile Takeover installs quickly and easily!

Now that you've unzipped the archive, take all the contents and drop them directly into your Blood directory. All the files have a "hos" prefix, making them group together in your folder for easy organization and searching. Nothing in Hostile Takeover will overwrite files in your current Blood directory, and will not alter the original game in any way. 

Hostile Takeover uses only the resources found in Blood (One Unit Whole Blood), which consists of the original game and the Plasma Pak. Cryptic Passage tiles and sounds are not used.


***************************************

Part III. Blood from Good Old Games (GOG.com) & Control / Audio Setup

***************************************

Installing and running Hostile Takeover using the Good Old Games version of One Unit Whole Blood
* by Lead QA Chris Hoopes (choopes@gmail.com) *

NOTE: The default installation directory for the GOG version of Blood on 64 bit Windows 7 is "C:\Program Files (x86)\GOG.com\One Unit Whole Blood"
We will be using that as a reference from here on out but if your install lies somewhere else please remember to update all paths mentioned to your own.

1) All files from inside of the Hostile Takeover zipped folder into the root Blood folder.  This means that all files go into "C:\Program Files (x86)\GOG.com\One Unit Whole Blood" or whatever your root directory, NOT "C:\Program Files (x86)\GOG.com\One Unit Whole Blood\Hostile Takeover".  If your files aren't in the root directory then it won't work.  Don't worry, nothing will be overwritten.

2) To enable cutscenes for the mod you may have to edit the hostile.ini file to reflect your install location. Refer to Blood.ini for the correct file path if the movies work properly for the original game.

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

While you're in Setup you'll also want to configure you're controls. You can rebind keyboard options within the game itself but mouse control must be set within Setup.  For a more modern control scheme click Setup Mouse and then make sure that Left Button is set to Weapon_Fire and Right Button is set to Weapon_Special_Fire.  This is of course entirely preferential but it's important to know where you can change this functionality.

You'll also want to set up your keyboard bindings as well.  The default controls are using the arrow keys to move, control to shoot, space to open doors, etc.  You'll need to change them either here in Setup or in-game to the more modern WASD movement scheme.

Now press Escape a few times to exit out of the Setup program and make sure to say YES to Save Setting Before Exiting.


5) Now you're ready to play!  In the Blood directory where you installed the Hostile Takeover files you should see a dosboxBloodhos.conf file.  This is the DOSBox configuration file that we'll use when running Death With.  These options allow for smooth fullscreen gaming and a few other nice things.

To launch the game using all of these options click the shortcut in your Blood folder called Hostile Takeover GOG.  If you look at the properties of this shortcut you'll notice that the target is set to:

"C:\Program Files (x86)\GOG.com\One Unit Whole Blood\DOSBOX\dosbox.exe" -conf dosboxBloodhos.conf -noconsole -c "exit"

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


Now at the end of your dosboxBloodhos.conf file edit the end so it looks like this:
quote:

    [autoexec]
    # Lines in this section will be run at startup.

    @ECHO OFF
    mount C "."
    imgmount D game.inst -t iso
    c:
    cls
    BMOUSE.EXE LAUNCH BLOOD.EXE -ini hostile.ini
    #hostile
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

Part IV. Play Hostile Takeover!

***************************************

The file hostile.bat will fire up Hostile Takeover! It follows this command:

blood -ini hostile.ini

This can be edited to suit your needs, just as the hostile.ini file can. You'll want to play Hostile Takeover through the .ini file to get the full experience (rather than playing them one-by-one in DOS), which includes music, on-screen messages, difficulty settings, etc.

If you are using DOSBox or a similar program, just navigate to your blood directory and type hostile