Ryandor's Dragon mod version 9
18 July 2002

New in this version:

Color:			"no-draw"
Color:			"see through" Cave Entrance
Transition:		Lava now working
Misc:			Fixed PaintShop Pro Palette file
Item Transition:	Dungeon House in Caves (disabled)
Misc:			Cleaned up some of the scripts
Misc:			Map Actions for Photoshop updated
Misc:			New FullMap using Mod 9 colors
Misc:			Map Piece modified to Mod 9 colors
Misc:			Fixed Fix Table

---

Lava: I've removed "lava -5" since it doesn't work in certain situations, however, it
is usable now. Make sure the surrounding tiles are the same altitude, otherwise statics tiles are off.

No-Draw: By request, this has been added.

Cave Entrance (see-through): This uses the no-draw tiles. If static floors are in the
entrance, you'll be able to see them.

Dungeon House in Caves: This creates walls and roofs in cave and dirt. Uses 1st set of
floorplates. (currently disabled due to bugs)

PaintShop Pro Palette file: it should now work. Please let me know if it does not.

example.bmp: this is an example map for use with mod 9. It includes most of the new
transitions. It's not perfect as I through it together real quick, but it can give you some ideas.

map pices: I've updated them to work with the mod 9 colortable

Fixed Fix Table: There is an internal error in Dragon in that it doesn't read this file correctly.
This is now fixed. Used to be X Y Z ID. Now it is X Y ID Z.

unevenly.txt: I commented this out since the example map doesn't need it

Dragon_m2b.exe: I've removed this since it's not useful for converting a map to bmp for converting back to a map.

---

About the Forest to swamp:
Gives the loook of a "sunken swamp" within a forest. Places a small "cliff" as an
edge. If your players need acces make sure you give access, otherwise the  
cliff will prevent access to the swamp. It is recomended to use this with "forest 5"
or higher altitude.

New Cave: Allows a different style cave wall and also has decorations.
With this transition you can now place caves in mountains, then manually edit the 
map0.mul, filling in the cave area with mountains. This will effectively hide your 
cave to be invisible in the Radar screen. Used in conjunction with Cave entrances, 
it is now possible to get caves into the map with a minimum of manual tweaking.
NOTE: The old cave.txt is still here for using of the ore carts and other decorations.
See my shots page on my web site for a preview.
(Credit to Dahr ek on http://home.t-online.de/home/mbgrinder/)

New Maptrans:
This optional file is for those with the newer version 1.05.00 pre-release of 
Dragon. The format is slightly different, but it will not work without it. Rename 
this to maptrans.txt to use. Do NOT use with Dragon 1.03.62

Map Actions and Brushes for Photoshop:
You will find instructions for use in readme-mapab.txt. Please read this.

About the Cave Entrances

Because of the way Dragon works, it will not place the correct tiles on
the "bottom row". This is due to the limitation of Dragon when it encounters 3
different types of tiles in a 3 x 3 area. However, final tweaks can be performed
after the map is finished being used with Dragon. Simply go to each location of
the cave entrances in WorldForge and fix the left and right bottom tiles of the
entrance. You could also use the fix file to do these automatically.

About the scripts

I felt it would be a good thing to include these as they are very useful.
The Misc script parts are for use in any area you like. Just copy and paste
them into the script that you want it in. Also, each script has comments with
each file. Read them.

About the  translation "grassbump"

This transition will place a "dirt cliff" similar to many areas in T2A. There are
limitations as to how you can use this new transition.
It only looks decent "below" other grass. To effectively use, paint a grass area at a
z of 5 or higher. Then paint a area (completely enclosed with the grass) with the
new color below the z of the grass.
Example: Area of "grass bump 0" surrounded by an areas of "grass 10"
Also, the color for grassbump has been changed for mod 7. When you apply the new
color table, it will adjust automatically.

=====

The Files:(*Updated for mod 9)

Filename                 Goes here                     Description
--------                 --------                      -----------
*maptrans.txt   	     /dragon/scripts               Used to translate the colors into the corect tile
maptrans105.txt		/dragon/scrpits			Used for Dragon 1.05.00 pre-release ONLY
*groups.txt     	     /dragon/scripts               Used for maptrans.txt
*betweentrans.txt        /dragon/scripts               Used for translation of tiles
*statbetweentrans.txt	/dragon/scripts			Used for translation of tiles
items.txt                /dragon/scripts               Used for determining statics placement
*furrows2grassb.txt		/dragon/scripts/map           New translation file
*furrows2grass.txt		/dragon/scripts/map           New translation file
*caveenti2mountian.txt	/dragon/scripts/map           New translation file
*grass2furrows.txt		/dragon/scripts/map           New translation file
*grassb2furrowns.txt	/dragon/scripts/map           New translation file
*grass2grassbump.txt     /dragon/scripts/map           New translation file
cave-ent2mountain.txt    /dragon/scripts/map           New translation file
forest2swamp.txt		/dragon/scripts/map			New translation file
cave2dirt.txt			/dragon/scripts/map			New translation file
black2dunnew.txt		/dragon/scripts/map			Fixed translation file
forest2swampb.txt		/dragon/scripts/statics		Statics file for forest to swamp
swamp2forestb.txt		/dragon/scripts/statics		Statics file for forest to swamp
black2caveRand.txt		/dragon/scripts/statics		Statics file for new cave
black2caveWalls.txt		/dragon/scripts/statics		Statics file for new cave
cave2blackRand.txt		/dragon/scripts/statics		Statics file for new cave
cave2blackWalls.txt		/dragon/scripts/statics		Statics file for new cave
*lava2mountain.txt 		/dragon/scripts/statics		Statics file for lava
*mountain2lava.txt		/dragon/scripts/statics		Statics file for lava
*lava2grass.txt 		/dragon/scripts/statics		Statics file for lava    
*grass2lava.txt     	/dragon/scripts/statics		Statics file for lava
*lava2forest.txt    	/dragon/scripts/statics		Statics file for lava
*forest2lava.txt    	/dragon/scripts/statics		Statics file for lava
*lava2desert.txt    	/dragon/scripts/statics		Statics file for lava
*desert2lava.txt    	/dragon/scripts/statics		Statics file for lava
*lava2snow.txt      	/dragon/scripts/statics		Statics file for lava (lave in snow???)
*snow2lava.txt      	/dragon/scripts/statics		Statics file for lava
*lava2jungle.txt    	/dragon/scripts/statics		Statics file for lava
*jungle2lava.txt    	/dragon/scripts/statics		Statics file for lava
*lava2dirt.txt      	/dragon/scripts/statics		Statics file for lava
*dirt2lava.txt      	/dragon/scripts/statics		Statics file for lava
*lava2swamp.txt     	/dragon/scripts/statics		Statics file for lava
*swamp2lava.txt     	/dragon/scripts/statics		Statics file for lava
*lava2star.txt      	/dragon/scripts/statics		Statics file for lava
*star2lava.txt      	/dragon/scripts/statics		Statics file for lava
*lava2cave.txt      	/dragon/scripts/statics		Statics file for lava
*cave2lava.txt      	/dragon/scripts/statics		Statics file for lava
*roof.txt               	/dragon/scripts/statics		Statics file house in cave
*roof2.txt              	/dragon/scripts/statics		Statics file house in cave
*stone2cave.txt         	/dragon/scripts/statics		Statics file house in cave
*cave2stone.txt         	/dragon/scripts/statics		Statics file house in cave
*rooftopfloor2.txt      	/dragon/scripts/statics		Statics file house in cave
jungle.txt			/dragon/scripts/items 		Item file
grass.txt                /dragon/scripts/items         Item file
grass2.txt               /dragon/scripts/items         Item file
alpine.txt               /dragon/scripts/items         Item file
cave.txt                 /dragon/scripts/items         Item file (not used, see note above)
cavenew.txt			/dragon/scripts/items         Item file
cavenewdeco.txt		/dragon/scripts/items         Item file
graveyard.txt            /dragon/scripts/items         Item file
miscitems.txt            /dragon/scripts/items         Item file
colortable_eng-mod.bmp   /dragon/addon                 Visual reference of colors used for map making
*dragon-mod.act 	     /dragon/addon                 Modified color table for map
*dragon-mod.aco		/dragon/addon				Adobe Photoshop Swatch file
*dragon-mod.pal		/dragon/addon				PaintShopPro Palette file
*readme.txt     	     /dragon/addon				This file
*mapactions.atn		/dragon/addon				Map Actions for Photoshop
mapbrushes.abr			/dragon/addon				Brushes for Photoshop
readme-mapab.txt		/dragon/addon				Readme file for Actions and Brushes
*example.bmp			/dragon/addon/full map		bmp example map
*example.fix			/dragon/addon/fixtable		Fixed FixTable

Backup your original (or previously modified) files if you want to keep them

If you are going to use this on an existing bmp, then these changes will require
corrections of older maps since the color table is changed from the original that
came with Dragon. You  should reapply all colors, by first: changing the color
table within Photoshop, then: repainting any colors that do not match corectly.
If you are starting a new bmp, then just use this color table as is. Just make
sure you apply the colortable to the new bmp. If you have any questions ICQ
or email me.

=====

**Revision history**

Mod 8: 17 Mar 2002
Misc:		Better organization of files
Color:		Starfield
Transition:	Forest to Swamp
Transition:	New cave
Transition:	Cave to Dirt
Transition:	Black to Dungeon (cave)
Script:		Jungle
Misc:		New maptrans for use with Dragon 1.05.00 (optional)
Misc:		PaintShopPro Palette file
Misc:		Map Actions and Brushes for Photoshop

Mod 7: 10 Feb 2002
Cave Entrances at altitute 20, 30 and 40
Item Scripts for Alpine and Graveyard (Credit to StormCrow in the forums at wwww.uocm.de)
Item Script for Cave
Misc Script Parts
Better readme.txt file

Mod 6: 25 Jan 2002
Addition translation "grassbump" (Credit to SickLab in the forums at wwww.uocm.de)

Mod 5: 12 Jan 2002
Changed the colors of the forest to be able to see better when painting grass next to forest.

Mod 4: 11 Dec 2001
Resorted the cave floor tiles due to getting confused too often. 

Mod 3: 21 Oct 2001
Added "water" altitudes of 20, 25, 30, 35, 40, 45, 50 (by request)

Mod 2: 15 Sept 2001
Modifications made:
	Adjustment to "cavewall"; moved to create space for consecutive "cave" colors
	Additions to "cave" (purple in color); added 5, 10, 15, 20, 25, 30
These changes will require corrections of older maps since the color table is changed.
Optionally, backup the original (or previously modified) files

Mod 1 :10 Sept 2001
Modifications made:
	Addition of "cave floor" altitutes of 5, 15, 25, 35
	Addition of "cavewall" altitutes of 30, 40, 50
	
=====

Credits

GM Merlin - For all the hard work he put into mod 9. I would not have had the time
to do everything that was done.
Dahr ek - Item and Statics Scripts http://home.t-online.de/home/mbgrinder/
HarcVohoc - Map Scripts
SickLab - Item Scripts
StormCrow - Item Scripts

=====

Questions, Comments and Suggestions

www.ryandor.com - Forums up and running! Post a message if you have problems.

ryandor@ryandor.com
ICQ:2006722 (use "About Dragon" when authorizing)
