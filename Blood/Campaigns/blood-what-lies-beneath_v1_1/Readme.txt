
BLOOD: WHAT LIES BENEATH V.1.1

======================================================================================================================================================================

CONTENTS:

1. CHANGELOG
2. INSTALLATION
3. SUPPORTED PORTS
4. WHY NOT OTHER PORTS?
5. WHAT ESLE TO SAY?
6. KNOWN BUGS
7. ASSET ACKNOWLEDGEMENTS


======================================================================================================================================================================

______________________________________________________________________________________________________________________________________________________________________

1. CHANGELOG
______________________________________________________________________________________________________________________________________________________________________

Version 1.1

- Updates Notblood.exe -> now the harpoon makes one hole on surfaces. BUT: savegames made with the previous version are incompatible
- Minor bug fixes in various maps
- Bug that rendered WLB22.MAP unbeatable on "well done" is fixed
- Timing related problems with switches on some maps are improved
- Fixed player freeze in WLB2X-maps when picking up mansion gate book
- Added more hints to the secret exit in WLB3.MAP and WLB4.MAP
- Changed book text in WLB3.MAP and WLB4.MAP to give more hints
- Changed book text in WLB7.MAP and WLB8.MAP to give more hints
- Various typos in the installer are corrected (sorry, changed the syntax quite a bit).
- Typos in blood.ini are gone
- LINUX support added (Please read the information in the installer and check it in the log-file)
- Source code of custom Nblood and NotBlood executables can be found here: https://drive.google.com/drive/folders/1q8qsPCYSRnZGCoPC602jRzjLPQO7a7Wb


______________________________________________________________________________________________________________________________________________________________________

2. INSTALLATION
______________________________________________________________________________________________________________________________________________________________________

To install "What Lies Beneath" just copy the files of this archive into your blood folder.
WLB doesn't override the blood resource files, it copies all necessary files into the "WLB" subfolder.
Just follow the WLB INSTALL.bat.

You have various options while installing. They all have to do with the amount of voxels that should be used and which source port you want to play with. 
If you have an older system I recommend NOT installing the voxel pack and installing "minimal voxels".

Installing FULL voxels (with the voxel pack) is only recommended fo BEEFY PCs!

After installation all files regarding the installation process will be deleted. If you want to re-install WLB please delete the WLB-folder and use the files within the downloaded archive again.
If any error occures during installation it will be documented in the logfile "WLBINST.LOG". Just open the file with a text editor and check it out.

______________________________________________________________________________________________________________________________________________________________________

3. SUPPORTED PORTS
______________________________________________________________________________________________________________________________________________________________________

WLB comes with a custom versions of nblood and notblood. This is at the moment the ONLY way you can play WLB!

Why?

-> This episode has more than 16 levels in the map list. "16" is a hardcoded maximum of levels in DOS blood. Every port has adapted this limit in the spririt of staying true to bloods roots.
-> I had to edit the source code of nblood and notblood to even make this episode playable.

If you run the addon via nblood/notblood you get a lot more modern animations and features within the levels. These modern touches are optional! The same levels can be run under DOS but they will work even without the modern features.

______________________________________________________________________________________________________________________________________________________________________

4. WHY NOT OTHER PORTS?______________________________________________________________________________________________________________________________________________________________________

As a guidline: There's of course the 16 map limit per episode in EVERY port. But there are other reason why they are not supported.


FRESH SUPPLY

This addon uses a lot of new assets (i.e. sounds, textures, voxels, animations...). To get WLB to run I have to modify the core resource files of Blood. 
Fresh Supply can't handle that well, if the core resource files are changed and the chances of a crash is highly likely.
A addon like "Deathwhish" does run because it uses only the original assets and doesn't cange anything except adding new maps.
So there is no way to get WLB to run on FS.

RAZE

Raze isn't fully compatable with the geomery handling of the OG build engine used in blood. Some tricks used in WLB (that work in DOS blood and every other soucre port) simply won't work in raze and you will get graphical glitches.
I've contacted the developers about this but this problem, but changing this would require a lot of rework of the code.
I tried to take a look at the source code of raze but had problems even compiling a custom version (noteworthy to mention is: I am NOT a programmer, I'm hanging in there as good as I can).
You can play the maps seperately in raze but expect graphical glitches here and there.

BUILDGDX

Has a high chance of crashing due to heavy xsprite use in the maps and there's the 16-level cap. But you can play the maps themselves without using the episode. Select the maps by choosing "user maps". The now available 1.17 version should work fine with the above mentioned xsprite problem but I don't have any experiecne with java to compile a version with 43 playable maps. If anyone wants to try this and gets the episode to run: I will add a functional version of BuildGDX to a new release version of WLB.

DOS

You can play the maps themselves in DOS by copying the dos files into wlb and typing "blood -map wlbXX" ["XX" is a placeholder for the map number]. But you CAN'T run the whole episode due to the hardcoded 16 maps limit. If there is demand for a DOS version I could do it and divide the whole 42 maps into 5 episodes but I'd have to cut some maps.
______________________________________________________________________________________________________________________________________________________________________

5. WHAT ESLE TO SAY?
______________________________________________________________________________________________________________________________________________________________________

This addon is NOT a linear addon for Blood (at least as non linear as I could make it on the original engine limits). On your journey you have choices to make that bring you to different paths. This means that there sometimes five different iterations of the same map necessary to achive this. So try another way next time.
______________________________________________________________________________________________________________________________________________________________________

6. KNOWN BUGS
______________________________________________________________________________________________________________________________________________________________________

RENDER-PROBLEMS:                If you enable all the voxel on weaker CPUs there can be a "ghosting effect" where voxels are rendered freely in the air.
                                Theses rendered voxels are bound to the player camera. Due to it beeing a render problem there's nothing I can do about it.
                                In this case I recommend playing with less voxels enabled.



WLB21.MAP and WLB23.MAP    ->   In both maps there are two big closed off room where you have to fight a lot of enemies to progress.
                                There's a chance that you will see this error message:

                                "Assertion failed: nSector >= 0 && nSector < kMaxSectors in file source/blood/src/db.cpp at line 222"

                                This only happened to me and some other play testers (not all of them; so maybe it's system dependent). It has something to
                                do with my edited executables. I think other sub-systems of nblood and notblood are struggeling with so many maps but I can't say for sure.

                                It occurs only by using a lot of explosives or a lit spray can. By now I have no idea why it happens or how to avoid it.
                                So please save at the beginning of these maps and at the beginning of a huge battle against a horde of enemies.
                                Sorry for the inconvenience.
______________________________________________________________________________________________________________________________________________________________________

7. ASSET ACKNOWLEDGEMENTS
______________________________________________________________________________________________________________________________________________________________________


Additional textures/sprites:

	Headfirst Productions
	Bethesda Softworks
	Probe Ldt.
	Gremlin interactive
	Shiny Entertainment
	Bungee
	Cyanide Studios
	Xatrix Entertainment
	Electronic Arts
	Lobotomy Software
	Sonic Team
	Cauldron
	3DRealms
	Monolith Productions
	nightsmoke
	LucasArts
	Lion Entertainment
	Raven Software
	Cranky Pants Games
	Valve Software
	Cyclone Studios
	Capcom
	Netherrealm Studios
	Gearbox Software
	DreamRift
	Intracorp
	SNK
	NextNinja
	Hartflip0218
	Lovecraft art by: zarono
	Hands model by: Dennis Haupt
        Doomguy model by: Mongee
	Chrono Trigger sprites by: SuperPhil64
	Computer sprites by: Wrim
	The Thing sprites by: Elendir



Additional voxels based on models/sprites/textures by:

	Headfirst Productions
	Cyanide Studios
	Ritual Entertainment
	Irrational Games
	Lion Entertainment
	Xatrix Entertainment
	Imagexcel
	Cranky Pants Games
	LucasArts
	Zoetrope Interactive
	Kindly Beast
	Black Forest Games
	Kindly Beast
	Fromsoft

Additional sounds/music by:

	Headfirst Productions
	Monolith Productions
	Capcom
	'Shipwrecked' remix by Luke Jansen
        (check him out at: www.youtube.com/@lukejansen3540)
	'Dark Carnival' remix by John S. Weekley
	'Great Temple' remix by John S. Weekley
	'Overlooked Hotel' remix by John S. Weekley
	'Lair of Shial' remix by John S. Weekley
	'Ghost Town' remix by John S. Weekley
	(check him out at: https://johnsweekley.bandcamp.com/)