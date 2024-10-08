---------------------------------------------------------------------------------
---------------------------------------------------------------------------------
-----																		-----
-----			ZikShadow Presents: NAM/NAPALM : Tangerine Edition			-----
-----																		-----
-----						Personal Set of Tweaks Addon					-----
-----																		-----
-----		Changes done here and there so I'll enjoy the game better.		-----
-----																		-----
-----				Maybe you will too. I don't know, I'm not you.			-----
-----																		-----
-----																		-----
---------------------------------------------------------------------------------
---------------------------------------------------------------------------------



------------------------
DESCRIPTION:
------------------------

For the longest time I've had an interest in a fair number of Vietnam War-based videogames. It's not everyday you see a videogame depicting a war where the protagonist (usually a US soldier, though there are some with NVA/Vietcong ones) inevitably loses at some point. Naturally as a result a game like NAM caught my attention not too long ago when I was informed of its existence. 

I tried playing it for 10 minutes, and promptly quit the game. It wasn't an enjoyable experience.

NAM is a game that strives to kick the player in the shins but often times without giving the player a chance to kick some shins themselves. And even without that in mind, it's dead obvious that the development team for this game had barely anything at all to work with. It looks and sounds like a glorified DN3D mod, trying too hard to be "realistic" without acknowledging the limitations of the engine and how it can severely affect one's enjoyment, giving barely any thoughts whether or not the experience is even remotely fair. Yes, I know, war is unfair, but videogames should be. To name all my grievances would be to write several paragraphs worth of basically the list below, so if you wanna know my list of complaints, imagine the list entries but they weren't implemented.

I was immensely annoyed with this game in many aspects, but at the same time I also find myself enjoying it in others. Which is why I decided out of the blue to start figuring out Build Engine modding from scratch in order to cobble up this little addon. Now, I will say, it's not much. I'm no expert Build modder, literally just started tinkering with stuff a few days ago. Don't expect a full remake of NAM or anything, but the changes here have made my experience with the game go so much better, and I figured I might as well release it for interested parties.

Now, about that list:



------------------------
LIST OF CHANGES (1.0):
------------------------

- Put hands on weapon sprites that initially didn't have them. M16, M72 LAW, M79, the works. JoeyTD redid the M16 hand to use the shotgun one instead, looks a bit more varied.
- Box added to the M60 sprite 'cause NAM does not have ammo tracking. If there's one pet peeve I have, it's seeing active ammo on the visible belt even though I have zero rounds.
- Take off ring from grenade 'cause there's no ring pulling animation and it'd be weird to throw an inactive grenade.
- Take off spoon from thrown grenade 'cause it's be weird to throw an inactive grenade.
- Replaced some sounds due to them not being punchy enough, or in the case of the flamethrower, too punchy to the point where it blares my ears everytime I use it. Also replaced sounds that are too noticeably from DN3D like falling grunts and others. Tried my best to keep the replacements about the same sound effect frequency as the OG game, 22khz. Most sounds are taken from Heart of Evil, though the flamethrower in particular is from They Hunger (Correction: After being informed, it seems that the original sound came from Team Fortress Classic, so I suppose Valve is to credit).
- Edited some existing sounds to add more impact to them. Using the medkit has an audible bandaging noise, for instance.
- All artillery armaments that aren't from the player is reduced in overall danger by half. Half radius, half damage, half everything. Should reduce the amount of cheap deaths from random explosions, though it will unfortunately reduce the effectiveness of requested airstrikes. Expect the enemy to have the same survival advantage.
- All disarmable mines are given 100% chance of succeeding a disarm attempt. Stepping on a landmine and not immediately moving is already a bridge far enough, so removing the random chance allowing players to absolutely disarm any mines they step on seems like a positive move.
- Most foliage sprites have been reduced in size by half in order to allow better visibility from the player. Considering how the enemy can already see you through props no prob, this was necessary to reduce being cheaply shot from far away behind several dozen thick grass decorations with X-Ray vision.
- Enemies have been given a distant firing sound that's audible from all distances. Done so that players can be aware that they're getting shot at and can act accordingly instead of doing so after being hit several times.
- Rewrote a fair amount of text stuff. Primary elements replaced are everything that says SPACE to instead use, well, USE. All weapon names have their proper designation, though ammo is kept the same for consistency. Clarified how the emplacements work. Stuff that sounds too techy like Holosoldier or Armorvest is replaced with Lifelike Puppet and Flakvest. Explained some of the mechanics in the item tags. The "Inventory Item" (renamed to just EQUIPMENT) tag now has listings for the percentages.
- The Remington Model 700 sniper rifle have been replaced to an M14. Yes, I know it was always supposed to be an M14 reading some stuff online, whoever sprited the world sprite for the original NAM sniper rifle sprited a polymer colored bolt action rifle instead of a primarily wood furniture gas-operated one with a magazine on it. In any case, the scope is useless anyways as NAM doesn't have zoom capabilities, so this replacement is done so the weapon could have more going on than just a boring black screen with some crosshairs slapped on. Nicked the Garand sprite from WWIIGI and slapped a magazine along with some poorly done overlays on top. Decent enough for government work.
- Replaced the machete sprites with Duke's recolored boot. Mainly done so quick kicking with other weapons don't look awful with 3 armed hooliganery. Yes, quick kicking is a valid strategy, especially if you're pumping your shotgun and the baddie in front of you isn't quite dead yet.
- Added one extra row of pixels on the mines specifically to contrast them better with the ground. Handwave reason being that those mines had to leave some dirt from the burial process.
- Recolored the chemical mine to look different from regular ones. Mainly 'cause of its mechanical difference in that it can't be disarmed, so it should look distinct to differentiate.
- Modified some item sprites that looked too DN3D-like to be slightly different. For example, the shotgun shell box has been recolored, Remington text changed to Winchester, and one of the shell on the right has been moved to the left. The armor was my edit of the original's sprite to look more flak vest-like instead of metal armor but green.
- Some textures that are too futuristic (unchanged from DN3D) like the teleporter and switches are given a slight makeover. Should be a bit more thematic.
- Recolored the portable medkit and added white outline to the red cross bit to better differentiate it with the regular non-portable medkits. Yes, I've unfortunately been a victim of accidentally picking up one thinking it's the other in the heat of combat.
- Increased the flamethrower range by twice the amount. Flamethrowers in 'Nam shoots napalm, not propane gas.
- Enemy shots emit ricochet sounds. Makes gunfights a bit louder, but atleast gives you more information that you're being shot at along with the distant shots.
- Edited all pain sounds to have a bit of impact noise. Might be not-so-noticeable in the heat of battle, but I still kept the lot anyways.
- Modified bouncing mine sprites to look more like the M16 mines. Actually is a bit harder to spot since I cut down on the thicker top bit to make the thin part, but atleast still has the dirt pixel row.



------------------------
LIST OF CHANGES (1.1):
------------------------

? Was planning to add a map of E1L6 to replace the map in that, well, map. The texture is used elsewhere unfortunately, so that didn't end up happening. Kept the texture incase I want to go with full map modifications in the future.
- Replaced the 4:3 menu stuff. Maybe not the intro, but everything from the episode end screen all the way to the help and credits screen are wide, now. Photos are replaced entirely with existing text modified on to be more concluding.
- Edited the looping cricket sound not have that incessant popping. Tried looping it a bit better.
- Weapon pickup sounds re-added. No player lines like in DN3D, just used the ammo pickup sound.
- Replaced the VC voices with ones from HoE. Not the Engrish ones, heavens no. Death sounds are less pronounced so they sound less uniform when you're strafing a group with the M60.
- Changed the emplacement system so you don't lose your ammobox the moment you stray a centimeter away from the emplacement. Changing carry item still does, though.
- Changed Equipment to Carry to shorten the text and allow me to expand the text a bit to inform players that some items could be used by crawling and hitting use at the same time.
- Modified both mounted M2HB and M60 sprites to lose the ammo belt. Considering you need an ammobox to use them in the first place, it'd be weird to see some ammo still in the gun.
- Modified M79 projectile to not look so oval thanks to just reusing the grenade sprites. Might have an effect on M16 mine cluster sprites as well.
- Modified US ammoboxes to have bold yellow letters and those high-low top covers compared to VC crates. The mortar ammobox in particular is now wooden.
- Modified Ithaca 37 view sprites to have the other half of the hand under the pump instead of above. Should be consistent with how Alan holds the gun.
- Modified M16's carry handle to look a bit more like an A1's instead of an A2's.



////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////



--------
CREDITS:
--------

Mod Author							: ZikShadow
Helped in Figuring Out Stuff		: Victorious_Games
99% of Sounds						: Heart of Evil Team
Flamethrower Sound					: Valve
Handed the M16						: JoeyTD
Removed the M16's wheel and lines	: ChopBlock223
Boots								: 3D Realms
M14									: TNT Team
Menu Photo							: Nightdive (taken from GOG page)
E1 End Photo						: iStock
E2 End Photo						: Pexels
Map Tally Photo						: Getty Images
Loadscreen Photo					: 123RF