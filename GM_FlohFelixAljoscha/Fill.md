1.1 Feature Type `dice: [[Fill#^FeatureNoLairs]]`

| dice: 1d20 | Result                                                                    |
| ---------- | ------------------------------------------------------------------------- |
| 1-4        | Geologic Feature `dice: [[Fill#^GeologicFeature]]` |
| 5-8        | Structure                                                                 |
| 9-12       | Resource                                                                  |
| 13         | Hazard                                                                    |
| 14         | Sign                                                                      |
| 15         | Dungeon                                                                   |
| 18         | Settlement                                                                |
| 20         | Magic                                                                     |
| 16-17      | Terrain                                                                   |
| 19         | Water                                                                     |
^FeatureNoLairs

#### Geologic

| dice: 1d6 | Result                                                                                                                                                                                                                                            |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1         | Change in Elevation. `dice: [[Fill#^hiLow]]` of `dice: [[Fill#^ElevationYards]]` `dice: [[Fill#^ElevationType]]`. The Area is `dice: [[Fill#^ElevationArea]]`. The Terrain is `dice: [[Fill#^elevationTerrain]]` comparing to surrounding Terrain |
| 2         | Soil                                                                                                                                                                                                                                              |
| 3         | Terrain                                                                                                                                                                                                                                           |
| 4         | Caves. The cave has `dice: [[Fill#^CaveEntrances]]`.One Entrance is `dice: [[Fill#^TypeCaveEntrance]]`. There are `dice: [[Fill#^NumberChambers]]`. Is the water in the cave? `dice: [[Fill#^caveWater]]`                                         |
| 5         | Rock                                                                                                                                                                                                                                              |
| 6         | Water                                                                                                                                                                                                                                             |
^GeologicFeature

##### Caves
Caves, obviously, are located below the ground and so are not always visible. Use the following rules to determine what the cave looks like. Note that any hex that has caves present gains the “Hazard (Sinkhole)” feature on a roll of 1 in 6 in the subhex containing the cave and the six subhexes around it. In addition, the vast majority of the time a cave system will be inhabited by a monster of some kind, even if it is not normally open to the surface world. There is a 1 in 20 chance per cave that it is totally uninhabited, with a further 1-3 in 6 chance that the cave is uninhabited for a specific reason (the air within is poisonous, the rock emits strong radiation, difficult to reach, etc.).

12-table-3.md

| d100   | Result               |
|:-------|:---------------------|
| 1-10   | no surface entrances |
| 11-50  | 1 entrance           |
| 51-75  | 2 entrances          |
| 76-90  | 3 entrances          |
| 91-99  | `dice: 1d4+2` entrances      |
| 100    | `dice: 2d4+2` entrances      |
^CaveEntrances

12-table-4.md

| d100   | Result                                                                                  |
|:-------|:----------------------------------------------------------------------------------------|
| 1-35   | "Classic" cave entrances                                                                |
| 36-70  | Existing sinkholes                                                                      |
| 71-85  | Concealed in some fashion (behind waterfall, heavy foliage, etc.)                       |
| 86-100 | Obviously worked (door fitted across entrance, carvings surrounding the entrance, etc.) |
^TypeCaveEntrance

Caves will have the following number of chambers. Add 5 to the roll for every entrance the cavern possesses beyond the first.

12-table-1.md

| d100   | Result         |
|:-------|:---------------|
| 1-40   | 1 chamber      |
| 41-60  | `dice: 1d4+1` chambers |
| 61-80  | `dice: 3d6` chambers   |
| 81-95  | `dice: 4d12` chambers  |
| 96-100 | `dice: 5d20` chambers  |
| 100+   | `dice: 6d100` chambers |
^NumberChambers

For every ten chambers in a cave there is a 1 in 6 chance the remaining chambers are treated as one level “deeper” (in terms of threats found in a dungeon of the same level). For every actual level a cave system possesses there is a cumulative 1% chance the system is connected to the mysterious subterranean world known as the “Underdark”.

Chambers in a cave are connected by tunnels. On a roll of 

| dice: 1d6 | Resut                                                  |
| --------- | ------------------------------------------------------ |
| 1-4       | the chambers are separated by normal dungeon distances |
| 5-6       | `dice: [[Fill#^ExtremeCaveDistances]]`                 |
^ChamberDistances

12-table-2.md


| d100   | Result              |
|:-------|:--------------------|
| 1-65   | `dice: 1d4`x100 yards apart |
| 66-90  | `dice: 4d6`x100 yards apart |
| 91-100 | `dice: 1d4` miles apart     |
^ExtremeCaveDistances

| dice: 1d6 | Result                                                                                                                                                                                                                                                                                                      |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-2       | dry. Dry caves are essentially dead and devoid of moisture; the moisture that created them has long vanished                                                                                                                                                                                                |
| 3-4       | wet.Wet caves are living; not only will they often have water sources, but the walls and ceiling are often coated with moisture and dissolved minerals.                                                                                                                                                     |
| 5         | dry and wet. Caves that are a combination of dry and wet should have these two microclimates separated based upon some kind of logical demarcation. Perhaps the underground river that formed the cavern system has cut its way down from the upper levels and can only be found further beneath the earth. |
| 6         | Formed not by water. t is also possible that a cave system has been created by other means: burrowing monsters such as purple worms, or extinct lava tubes, or the intrusion of elemental planes into the material are all possible sources for the creation of unique cave systems.                        |
^caveWater

Caves will be dry (1-2), wet (3-4), a combination of the two (5), or formed through different means (6). Dry caves are essentially dead and devoid of moisture; the moisture that created them has long vanished. Wet caves are living; not only will they often have water sources, but the walls and ceiling are often coated with moisture and dissolved minerals.

Caves that are a combination of dry and wet should have these two microclimates separated based upon some kind of logical demarcation. Perhaps the underground river that formed the cavern system has cut its way down from the upper levels and can only be found further beneath the earth.

It is also possible that a cave system has been created by other means: burrowing monsters such as purple worms, or extinct lava tubes, or the intrusion of elemental planes into the material are all possible sources for the creation of unique cave systems.

Use the Dungeon Stocking Table on p. 225 of OSE core to determine what is present in a cave system. As a rule of thumb, caves of 1-4 chambers will generally be inhabited by only a single type of monster (whether goblins, mountain lions, etc.). Larger caves will be populated as dungeons, with multiple and diverse populations.

#### Change in Elevation
The terrain in a given area is at a different elevation than the surrounding land. This can be hill, butte, plateau, valley, holler, sinkhole, or other descriptive term.


| dice: 1d2 | result     |
| --------- | ---------- |
| 1         | elevation  |
| 2         | depression |
^hiLow


13-table-1.md

| d100   | Result                                                                                                                                                                                                                        |
|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-75   | The change is natural, the result of time and the elements.                                                                                                                                                                   |
| 76-90  | The change is natural but out of place or the result  of  natural  violence;  a  rock  formation that  does  not  belong  in  the  area,  a  gorge formed not by the slow erosion from a river but an active fault line, etc. |
| 91-96  | The change is unnatural but clearly the work of years of physical labor.                                                                                                                                                      |
| 97-100 | The change is unnatural and clearly the work of magic.                                                                                                                                                                        |
^ElevationType


The elevation will be higher (1-3) or lower (4-6) than the surrounding land.

13-table-4.md

| d100   | Result                                                                        |
|:------ |:----------------------------------------------------------------------------- |
| 1-50   | The land is `dice: 5d20` yards lower or higher than the surrounding area.     |
| 51-75  | The land is `dice: 10d20` yards lower or higher than the surrounding area.    |
| 76-100 | The land is `dice: 1d10`×100 yards lower or higher than the surrounding area. |

^ElevationYards



Change in Elevation Comprises...

13-table-5.md

| d100   | Result                    |
|:------ |:------------------------- |
| 1-35   | a single subhex           |
| 36-70  | `dice: 1d4+1` subhexes    |
| 71-85  | `dice: 3d4` subhexes      |
| 86-98  | `dice: 4d8` subhexes      |
| 99-100 | `dice: 1d4+1` total hexes |
^ElevationArea

There is a 1-4 in 6 chance that the change in elevation represents a differing terrain type than the surrounding environs. This change in terrain will most often (1-4 in 6) be within one degree of the surrounding terrain or (5-6) within two degrees (see Terrain, p. 55 below).

| dice: 1d100 | Result                        |
| ----------- | ----------------------------- |
| 1-44        | Different Terrain one degree  |
| 45-66       | Different Terrain two degrees |
| 71-100      | same Terrain                  |
^elevationTerrain

#### Rocks
The terrain is unusually rocky. This manifests itself in three different ways:

13-table-2.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|:------ |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1-35   | A  number  of  smaller  rocks  (roll  `dice: 1d6`-1  to indicate the average diameter, in feet), with a  density  of  `dice: 3d10`  per  `dice: 1d20`×100  sq.  ft.  A result of 0 indicates the rocks are, on average, smaller than a foot in diameter.`dice: [[Fill#^AreaRocks]]`                                                                                                                                                                                                   |
| 36-70  | a  smaller  number  of  larger  rocks,  with  an average diameter of 3d6 feet and a density of 1d4 per 1d20×100 feet. `dice: [[Fill#^AreaRocks]]`                                                                                                                                                                                                                                                                                                             |
| 71-100 | an  outcropping  of  rock.  If  the  outcropping occupies  a  single  subhex  there  is  only  one; if  multiple  subhexes  there  is  a  chance  each subhex will have (1-3) a single outcropping, (4-5) 1d4 outcroppings (depending on overall  size),  or  (6)  the  outcroppings  join together  to  form  one  massive  outcropping that covers the entire area.  To determine the size of the outcropping roll below: `dice: [[Fill#^OutcroppingSize]]` |
^typeRocks

size of Outcropping
13-table-3.md

| d100   | Result                                                  |
|:-------|:--------------------------------------------------------|
| 1-25   | `dice: 1d10`×1000 sq. ft. (approx. 75 feet to a side)           |
| 26-50  | `dice: 1d10`×10000 sq. ft (approx. 230 feet to a side)          |
| 51-75  | `dice: 1d10`×100000  sq.  ft.  (approx.  715  feet  to  a side) |
| 76-100 | `dice: 1d10`×1000000 sq. ft (2,400 feet to a side)              |
^OutcroppingSize

Area of Outcopping
13-table-6.md

| d100   | Result         |
|:-------|:---------------|
| 1-60   | 1 subhex       |
| 61-89  | `dice: 1d4+1` subhexes |
| 90-96  | `dice: 3d8` subhexes   |
| 97-99  | 1 hex          |
| 100    | `dice: 1d4+1` hexes    |
^OutcroppingArea

If the rocks are not an outcropping they will cover an area of . . .
14-table-1.md

| d100   | Result                  |
|:-------|:------------------------|
| 1-30   | `dice: 1d4`x100 square feet     |
| 31-50  | `dice: 2d6`x500 square feet     |
| 51-65  | `dice: 3d8`x1,000 square feet   |
| 66-80  | `dice: 4d10`x10,000 square feet |
| 81-90  | `dice: 1d4` subhexes            |
| 91-95  | `dice: 3d6` subhexes            |
| 96-99  | `dice: 4d8` subhexes            |
| 100    | `dice: 1d4` hexes               |
^AreaRocks
The rocks will be . .
14-table-2.md

| d100   | Result                                                                                                                                                        |
|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-60   | Naturally  occurring,  the  result  of  erosion, weathering, etc.                                                                                             |
| 61-95  | Naturally occurring, but not usually found in the area (such as the rocks deposited by glacier)                                                               |
| 96-100 | Not  naturally  occurring.   They  will  be deliberately placed, trolls turned to stone by the sun’s rays, petrified tree stumps from an ancient forest, etc. |
^OriginRocks


The Referee can refer to the Resources section on p. 37 to determine the type of rock.

There’s an additional 1 in 6 chance of something unusual about the rocks . . .
(1-3) The rocks have been written on. The writing is 
	1. 1-2 carved into the stone, 
	2. 3-4 written on the surface with some substance, 
	3. 5 patterned in lichen or moss, or 
	4. 6 appears organically in the surface of the rock itself. 
- Further, the writing will either be on a single stone (1-3), 1d20+1 stones (4-5) or all of the stones (6) 
The writing 
1.  Is meaningless, obscene or pornographic graffiti.
2.  Contains the formula to a spell (1-4) or magical item (5-6). It takes 1d8 weeks plus one day per additional stone containing the writing to decipher and understand what is scribed upon it.
3.  A prophecy, concerning events that are yet to come (1-4) or have already passed (5-6). There’s a 1-2 in 6 chance the prophecy is wrong.
4.  A map. On a 1-2 it’s a treasure map (roll on the Scrolls treasure table, treating all non treasure map results as a reroll), 3-4 it’s a map of the surrounding area, 5 it’s a map to an undiscovered/unknown area (1-2 in 6 chance of being in another plane or dimension), or 6 a map of a random location.
5.  There’s a small crevice in the rock, and if the adventurers write a question on a slip of paper (1-2 in 6 chance that the question must be asked in a specific language, (3-4) written in the asker’s blood, or (5-6) accompanied by a gift), slip it into the crevice, and return the next day the writing will reform itself as an answer to the question posed (treat as 1-3 augury, 4-5 divination, or 6 commune, all as if cast by a cleric of level 6+1d8).
6.  The writing is 1 a record of historical events (see Monuments, p. 17), 2 a warning about dangers (1-4 current, 5-6 past and no longer relevant) in the area, 3 a personal missive directed to one of the adventurers (1-3 chance of being accurate, from a dead relative or friend. There’s a 1-2 chance it will contain advice about upcoming events, otherwise it will just be the friend or relative saying hello), 4 a single letter per stone (see above to determine the number of stones with writing on them), arranged in a random fashion (the letters, when sorted, spell out 1-2 a dirty word, 3-4 the name of an ancient king or magician, 5 the name of an ally of the party who means to betray them, or 6 the true name of a demon or fairy that can be used to bind said creature), 5 assembly directions (if the stones are arranged according to the directions written upon them they will create 1-2 a sculpture, 3-4 a crude dwelling, 5 a portal that functions as a gate to another world, or 6 a circle 1d20+10 feet in diameter, inside which the adventurers may camp without fear of wandering monsters. In the last two instances the effects last for 1 1d4 uses (camping 8 hours counts as a “use”), 2 1d4 hours, 3 3d4 hours, 4 1d4 days, 5 1d4 weeks, 6 permanently) or 6 something else of the Referee’s choosing.
4-5) The rocks are arranged in a specific pattern. The pattern can
- 1-4 only be discerned from above or 
- 5-6 is obvious from ground level. The pattern will be one of the following . . .
	- The pattern is of a random shape or arrangement, determined by the whim of of a mad artist, whimsical deity or capricious spirit.
	- The pattern is mundane in nature, forming a shape or image with little to no significance except to its executor.
	- There is power within the pattern, but it is not clear what it is. It takes 1d8 days of study to determine what the pattern does. The pattern is 
		- 1 a ward against something (roll on the Scrolls table to determine what it wards against), 
		- 2 functions as a gate (
			- 1-3 to another place in this world, 
			- 4-5 to a place in another world or dimension, or 
			- 6 to another time), 
		- 3 functions to alter the surrounding weather (
			- 1-2 by moderating, 
			- 3-4 by intensifying, or 
			- 5-6 by attracting a certain phenomenon), 
		- 4 it acts as a prison, containing a powerful creature or creatures (with a combined HD total of 10d10)
		- 5 acts as a focus for ley line energy (see the section on Magic, p. 66, as well as Hex 13.22 for more information on ley lines. There’s a 1-3 in 6 chance the ley line it once focused has since shifted position), or 
		- 6 is an artifact designed to cast a permanent spell over a larger area.
(6) The Rocks are Magical. Refer to the section on Magical Features.

##### Soil
15-table-1.md

| d6   | Result                                                                                                                                                                                                                                                        |
|:-----|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-3  | The soil has the special quality due to a mineral, nutrient or other naturally occurring feature.                                                                                                                                                             |
| 4-5  | The soil is different because of artificial means (perhaps it is terraced or fertilized or has been poisoned  by  an  enemy).  If  this  is  the  case, further  labor  can  altered  it  from  its  current state at a cost of 1,000 gp per subhex affected. |
| 6    | The soil is as it is as the result of a curse or beneficial  spell.  It  is  possible  to  remove  the curse or spell.                                                                                                                                        |


17-table-1.md

| d100   | Result       |
|:-------|:-------------|
| 1-30   | Single Grace |
| 31-60  | 1d4+1 dead   |
| 61-75  | 3d4 dead     |
| 76-85  | 4d6 dead     |
| 86-96  | 5d10 dead    |
| 96-97  | 6d20 dead    |
| 98     | 7d100 dead   |
| 99     | 10d100       |
| 100    | 100d100 dead |


17-table-2.md

| d100   | Result         |
|:-------|:---------------|
| 1      | Burial Grounds |
| 2      | Monuments      |
| 3-5    | Dwellings      |
| 6      | Fortificaton   |
| 7-8    | Infrastructure |
| 9      | Barriers       |
| 10     | Dungeons       |


18-table-1.md

| d100                | Result                                    |
|:--------------------|:------------------------------------------|
| 1-50                | Human (or whatever the dominant race is.) |
| 51-75               | Demi-human (elf, dwarf, gnome, etc.)      |
| 76-90               | Humanoid                                  |
| 91-95               | Monster                                   |
| 96-100 Mix of races |                                           |


18-table-2.md

| d100   | Result                                                                                           |
|:-------|:-------------------------------------------------------------------------------------------------|
| 1-25   | They’re not.  The dead are left exposed to the elements as they fell.                            |
| 36-30  | Buried in a mass grave                                                                           |
| 31-60  | Wooden markers                                                                                   |
| 61-75  | Stone tombstones                                                                                 |
| 76-80  | Mausoleums or crypts                                                                             |
| 81-86  | Barrows or burial mounds                                                                         |
| 87-90  | Ritually exposed to the elements                                                                 |
| 91-95  | As punishment (gibbets, crucifixion, gallows, etc.)                                              |
| 96-99  | In unmarked graves.                                                                              |
| 100    | Unique or magically (turned to stone or trees, frozen in blocks of ice, embedded in amber, etc.) |


18-table-3.md

| d100   | Result        |
|:-------|:--------------|
| 1-5    | 1d4 days      |
| 6-10   | 1d4 weeks     |
| 11-20  | 1d12 months   |
| 21-30  | 1d10 years    |
| 31-40  | 2d20 years    |
| 41-50  | 5d20 years    |
| 51-75  | 10d20 years   |
| 76-99  | 10d100 years  |
| 100    | 1d4 millennia |


20-table-1.md

| d100   | Result                            |
|:-------|:----------------------------------|
| 1-40   | Humans                            |
| 41-75  | Demi-humans                       |
| 76-90  | Humanoids                         |
| 91-98  | Other Races (dragon, giant, etc.) |
| 99-100 | Abstract concepts                 |


20-table-2.md

| d100   | Result                                                                                                           |
|:-------|:-----------------------------------------------------------------------------------------------------------------|
| 1-25   | Built  to  honor  the  dead  (usually  fallen  in battle or disaster)                                            |
| 26-50  | Built to honor an event (such as a battle, the signing of a treaty, the birth of a ruler, etc.).                 |
| 51-75  | Built to honor an individual (such as a ruler, powerful mage, etc.)                                              |
| 76-85  | Built to honor a concept (such as Law or Chaos)                                                                  |
| 86-95  | Built to honor a religion or deity. Refer to the section on shrines on p. 34                                     |
| 96-100 | Built  to  house  an  object  or  person  (such as  an  artifact  or  relic,  or  an  emperor’s burial chambers) |


20-table-3.md

| d100   | Result                                                             |
|:------ |:------------------------------------------------------------------ |
| 1-25   | A statue (1-4) or multiple statues (5-6)                           |
| 26-50  | An obelisk (1-3) or column (4-6)                                   |
| 51-75  | Megalith                                                           |
| 76-85  | Arch (1-3), building (4-5) or freeform structure (6)               |
| 86-90  | Pyramid  (1-2),  terraced  pyramid  (3-4)  or earthen mounds (5-6) |
| 91-95  | Fountain or Water feature (refer to p. 28)                         |
| 96-100 | Magical or Unique material/form                                    |


21-table-1.md

| d12   | Result   |
|:------|:---------|
| 1-2   | Level 1  |
| 3-4   | Level 2  |
| 5-6   | Level 3* |
| 7     | Level 4  |
| 8     | Level 5* |
| 9     | Level 5  |
| 10    | Level 7* |
| 11    | Level 8  |
| 12    | Level 9* |


21-table-2.md

| d100   | Result        |
|:-------|:--------------|
| 1-10   | 1d10 years    |
| 11-50  | 10d10 years   |
| 51-95  | 10d100 years  |
| 96-100 | 10d1000 years |


21-table-3.md

| d100   | Result                                                                                                                                                                                                                                                                       |
|:-------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1      | Small. probably erected by a race of Micronians or perhaps awakened animals.                                                                                                                                                                                                 |
| 2-60   | Medium. sized or scaled for Men (statues will be approximately human height, buildings and other structures scaled for human habitation).                                                                                                                                    |
| 61-90  | Large. sized for ogres and such. Statues will be approximately 8-10’ tall, obelisks around 20-35 feet. There is a 1-2 in 6 chance that the monuments are actually designed by a large race; the other 66% of the time they’re built by human-sized creatures with big ideas. |
| 91-99  | Giant-sized.  Statues  will  be  approximately 11-20’ tall,  obelisks  and  columns  around 36-50 feet. There is a 1 in 6 chance that the monuments are actually designed by a large race;  the  rest  of  the  time  they’re  built  by human-sized folks with big ideas.   |
| 100    | Enormous.  These  monuments  are  so  large they boggle the mind and are either built by creatures larger than the largest giants (1 in 6 chance) or by large kingdoms and empires (such as the Pyramids at Giza).                                                           |


21-table-4.md

| d100   | Result           |
|:-------|:-----------------|
| 1-20   | Wood/Bone/Brick  |
| 21-45  | Metal            |
| 46-95  | Stone            |
| 96-100 | Exotic Materials |


22-table-1.md

| d100   | Result                                                                                                                                                                                                                                   |
|:-------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-25   | Inhabited by monsters. Roll on the wandering encounter  table  appropriate  for  the  area  to determine exactly what lives within.                                                                                                      |
| 26-60  | Uninhabited. If it is uninhabited there is a 1-2 in 6 chance of there being valuables within the house, with the following treasure type (1-A, 2-B, 3-C, 4-D, 5-E, 6-F). There is an additional 1-3 in 6 chance the treasure is trapped. |
| 61-100 | Inhabited  by the  original  builders (or the descendants/same race as the original builders).                                                                                                                                           |


22-table-2.md

| d100   | Result        |
|:-------|:--------------|
| 1-10   | 1d10 years    |
| 11-60  | 10d10 years   |
| 61-99  | 10d100 years  |
| 100    | 10d1000 years |


22-table-3.md

| d100   | Result                       |
|:-------|:-----------------------------|
| 1-15   | Crumbling and falling apart. |
| 16-50  | In need of some repair.      |
| 51-85  | In relatively decent shape.  |
| 86-100 | Immaculately maintained.     |


22-table-4.md

| d100   | Result                                                                                 |
|:-------|:---------------------------------------------------------------------------------------|
| 1-25   | Materials  found  locally  and  appropriate  for the surroundings.                     |
| 26-60  | Materials imported from afar.                                                          |
| 61-100 | Unique materials or those created by magic: a palace of glass, or amber, for instance. |


23-table-1.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 96-98  | Very Large. The dwelling has 1d12+5 rooms and  is  roughly  the  size  of  a  manor  house. There’s  a  1-3 in  6  chance that there  are 1d2+1  outbuildings  surrounding  the  main house,  with  2d4  rooms  divided  amongst them. There’s a 1-3 in 6 chance the buildings are  surrounded  by  walls  or  other  defensive fortifications,  and  an  additional  1-2 in  8 chance the building is actually a keep, with a primarily defensive function. |
| 99-100 | Palatial. The dwelling has 2d20+5 rooms and is roughly the size of a castle. There’s a 1-4 in 8 chance that it actually is a castle. There’s an additional 1-3 in 6 chance that there are 2d4 outbuildings, with 4d4 rooms between them. If the structure is not a castle or keep there’s a 1-3 in 6 chance the buildings are surrounded by walls or similar fortifications.                                                                                 |


23-table-2.md

| d100   | Result        |
|:-------|:--------------|
| 1-10   | 1d10 years    |
| 11-60  | 10d10 years   |
| 61-99  | 10d100 years  |
| 100    | 10d1000 years |


23-table-3.md

| d100   | Result                       |
|:-------|:-----------------------------|
| 1-15   | Crumbling and falling apart. |
| 16-50  | In need of some repair.      |
| 51-85  | In relatively decent shape.  |
| 86-100 | Immaculately maintained.     |


23-table-4.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-10   | Tiny.  A  single-room  hut,  hovel  or  house. There’s  a  1-2  in  6  chance  the  dwelling  was designed to be temporary (such as a lean-to, hide tent, yurt, etc.). It’s been built to provide shelter, with no extraneous rooms.                                                                                                                                                                                                                                                                                                            |
| 11-30  | Small.  The dwelling has 1d3 rooms, potentially  with  a  sleeping  space  separate from the living space. There’s a 1 in 6 chance the  dwelling is  surrounded  by  a  wall  or similar fortification.                                                                                                                                                                                                                                                                                                                                         |
| 31-75  | Medium.  The  dwelling  has  1d4+1  rooms and  is  generally  what  we  would  consider to  be  a  “house”  with  dedicated  rooms  for different purposes. There’s a 1-2 in 6 chance the  dwelling is  surrounded  by  a  wall  or similar fortification. There’s a 1 in 8 chance the dwelling is actually a fortified keep.                                                                                                                                                                                                                   |
| 76-95  | Large.  The  dwelling  has  1d6+4  rooms  and would  be  consistent  with  a large freehold supporting  several  families.  If  there  are  more than 6 rooms there’s a 1-2 in 6 chance the rooms are  actually  divided  between  1d2+1  buildings, forming a compound. If all the rooms are in one building, there’s a 1-2 in 6 chance the dwelling is surrounded by a wall, or if in multiple buildings there’s a 1-3 in 6 chance of the same. There’s a 1 in 8 chance the building is actually a keep, with a primarily defensive function. |


24-table-1.md

| d100   | Result                                                                                                                                                                                                                                              |
|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-10   | 2d20 feet.                                                                                                                                                                                                                                          |
| 11-25  | 8d20 feet. Walls of this length have a 1-2 in 6 chance of having a gate or opening along the length.                                                                                                                                                |
| 26-65  | 8d100 feet. Walls of this length have a 1-3 in 6  chance  of  having  a  gate  or  opening  every 1d4×100 feet. If the wall is taller than 10’ there is a 1-2 in 6 chance there is a tower or other defensive structure located every 1d6×100 feet. |
| 66-75  | 8d100×10 feet. See above.                                                                                                                                                                                                                           |
| 76-85  | 1d6 miles. See above.                                                                                                                                                                                                                               |
| 86-96  | 3d4 miles. See above.                                                                                                                                                                                                                               |
| 97-99  | 5d20 miles. See above.                                                                                                                                                                                                                              |
| 100    | 100+ miles long. See above                                                                                                                                                                                                                          |


24-table-2.md

| d100   | Result                                                                                                                                                                      |
|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-40   | Earth.  Typically  these  will  be  the  simplest kinds of fortifications: earthen berms behind which troops can hide, trenches dug into the earth lined with spikes, etc.  |
| 41-70  | Wood.  The  fortifications  will  be  primarily constructed  of  wood  and  will  be  either  a palisade, a hastily erected wall, a fort framed from massive logs, etc.     |
| 71-90  | Stone. These  could  be  a  stone  wall  snaking across  the  terrain,  a  granite  redoubt  carved into  living  rock  or  a  keep  perched  atop  a lonely tor.           |
| 91-98  | Exotic Material. The defensive structure will be built out of some sort of exotic material, that  may  or  may  not  have  been  created  or crafted through mundane means. |
| 99-100 | Magical Material. The defensive structure is clearly magical in nature: a wall of flame, or corpses, or a castle made from ice.                                             |


24-table-3.md

| d100   | Result    |
|:-------|:----------|
| 1-20   | Wall.     |
| 21-40  | Hillfort. |
| 41-55  | Berm.     |
| 56-75  | Trench.   |
| 76-85  | Tower.    |
| 86-95  | Keep.     |
| 96-100 | Castle.   |


25-table-1.md

| d100   | Result                                                                                                                                                                                                                                                                                                            |
|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-20   | Encompasses  1d10×1,000  sq.  ft.  Has  one “terrace”  with  ramparts  1d6+4  feet  tall  and one entrance.                                                                                                                                                                                                       |
| 21-60  | Encompasses  1d100×1,000  sq.  ft.  Has  one terrace with ramparts 1d6+6 feet tall and one entrance.                                                                                                                                                                                                              |
| 61-90  | Encompasses  1d10×10,000  sq.  ft.  Has  one terrace  if  under  90,000  sq.  ft.,  two  terraces if over that. The ramparts will be 1d6+6 feet tall, with 1d2 entrances per terrace.                                                                                                                             |
| 91-99  | Encompasses 1d100×10,000 sq. ft.  Has 1d2+1  terraces,  with  ramparts  1d8+7  feet tall, and 1d3 entrances per terrace.                                                                                                                                                                                          |
| 100    | Encompasses 3d100×10,000 sq. ft.  Has 1d3+1  terraces,  with  ramparts  1d8+7  feet tall, and 1d4 entrances per terrace. Hillforts encompassing more than 2,000,000 sq. ft. are largely useless as defensive structures and are instead used  for more pedestrian purposes, such as the containment of livestock. |


25-table-2.md

| d100   | Result                                                                                                                                                                                                                                                       |
|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-10   | 2d20 feet                                                                                                                                                                                                                                                    |
| 11-45  | 8d20  feet.  Berms  this  long  have  a  1-3  in  6 chance of having a single break somewhere along the line to allow passage.                                                                                                                               |
| 46-65  | 8d100 feet long. Berms this long have a 1-3 in 6 chance of having a gate or opening every 1d4×100  feet.  If  the  berm  is  taller  than  10’ there  is  a  1  in  6  chance  there  is  a  tower  or other defensive structure located every 1d6×100 feet. |
| 66-75  | 8d100×10 feet. See above.                                                                                                                                                                                                                                    |
| 76-85  | 1d6 miles. See above.                                                                                                                                                                                                                                        |
| 86-96  | 3d4 miles. See above.                                                                                                                                                                                                                                        |
| 97-99  | 5d20 miles. See above.                                                                                                                                                                                                                                       |
| 100    | 100+ miles long. See above.                                                                                                                                                                                                                                  |


25-table-3.md

| d100   | Result            |
|:-------|:------------------|
| 1-25   | 1d4+4 feet tall   |
| 26-86  | 1d6+8 feet tall   |
| 87-99  | 1d12+12 feet tall |
| 100    | 1d20+20 feet tall |


25-table-4.md

| d100   | Result          |
|:-------|:----------------|
| 1-10   | 1d10 months old |
| 11-60  | 1d10 years old  |
| 61-99  | 10d10 years     |
| 100    | 10d100 years    |


26-table-1.md

| d100   | Result        |
|:-------|:--------------|
| 1-10   | 1d10 years    |
| 11-60  | 10d10 years   |
| 61-99  | 10d100 years  |
| 100    | 10d1000 years |


26-table-2.md

| d100   | Result                       |
|:-------|:-----------------------------|
| 1-15   | Crumbling and falling apart. |
| 16-50  | In need of some repair.      |
| 51-85  | In relatively decent shape.  |
| 86-100 | Immaculately maintained.     |


26-table-3.md

| d20   | Result     |
|:------|:-----------|
| 1-8   | Roads      |
| 9-15  | Water      |
| 16-20 | Commercial |


26-table-4.md

| d100   | Result                                                                                                                                         |
|:-------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
| 1-30   | Wood.  The  structures  are  made  of  worked wood,  limiting  their  size  to  no  more  than four stories tall (approximately 50 feet high). |
| 31-80  | Stone. Built primarily of stone, these structures have a size limited to eight stories (approximately 100 feet high).                          |
| 81-100 | Exotic.  Built  from  exotic  materials  or  with the aid of magic, towers may be carved from living trees, or glass.                          |


26-table-5.md

| d100                                   | Result                                                                                                                         |
|:---------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------|
| 1-30                                   | Dirt.  Dirt  roads  do  not  grant  the  bonus  to movement  (see  p.  111,  OSE  core)  during rain, or for 1d3–1 days after. |
| 31-60                                  | Paved with dry laid stones (1-3) or bricks (4-6).                                                                              |
| 61-90                                  | Wood (logs laid side by side), a “plank road”.                                                                                 |
| 91-98                                  | Artificial (such as Roman concrete roads).                                                                                     |
| 99-100 Magical or unusual (see below). |                                                                                                                                |


27-table-1.md

| d10 | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|:--- |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1-3 | Unique material. The road is built of an unusual material. The road is made from (1) one of the materials above, but unique or rare to the region, (2) iron, (3) bone, (4) graves, (5) glass, (6) high-tech material like plastic or concrete, (7) ceramics, (8) living material, (9-10) other.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| 4-6 | Unique construction. The road is built in an unusual manner. It is (1) elevated, (2) sunken, (3) covered, (4) hidden, (5) goes underground for a portion, (6) other.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| 7   | Magical (benign). The road is enchanted in a manner that is beneficial to those traveling on it. It (1) is safer than normal. Wandering monster chances are reduced by 1d2 while on the road, (2) those on the road are under the effects of a permanent protection from evil spell, (3) food does not spoil or go bad while on the road, (4) travelers on the road move faster than normal: if granted, the normal 50% bonus to movement is increased to 75%, or if not granted travelers have a 25% bonus, (5) travelers on the road do not incur exhaustion for forced marching, (6) healing is increased: roll twice for all healing spells and effects and take the better of two results, (7) all travelers on the road are able to understand any spoken language, or (8) other.                                                                                                                                                                                                                                                                                                                |
| 8   | Magical (malign). The road is enchanted in a manner that is dangerous to those traveling on it. (1) It is more dangerous than normal: those traveling on the road have their chances of wandering monsters increased by 1d2, (2) normal rations spoil after a day on the road and iron rations after 1d4 days, (3) movement is slowed: if a speed bonus would normally be granted for maintained roads it is lost, and if not movement is 50% slower, (4) turning undead is less potent: if attempting to turn undead within 50’ of the road roll twice, taking the lower result, (5) sleep within 50’ of the road is fitful, and does not count as rest for purposes of memorizing spells or avoiding exhaustion, (6) healing magics are minimized: roll twice when determining damage healed, taking the lower of the two results, (7) creatures slain on the road are either (1-2 incapable of being raised or brought back to life, short of a wish spell, or 3-6 raised as undead within 1d8 days of their death; they will be 1-2 skeletons, 3-4 zombies, 5 wights, or 6 wraiths), or (8) other. |
| 9-10  | Magical  (neutral).  The  road  possesses  an enchantment that is neither directly beneficial nor malignant. It is (1) a pathway to another place  (1-4)  or  plane  of  existence  (5-6),  (2) can  only  be  traveled  on  by  those  who  know the  proper  words  (1-3)  or  carry  the  correct charms  (4-6),  (3)  the  road  is  lit  by  floating magical  lights:  there’s  a  1-2  in  6  chance  the lights  only  illuminate  when  living  creatures are within 30’, otherwise they stay lit, (4) the road is intelligent, inhabited by an animating spirit;  it  is  1-2  Lawful,  3-6  Neutral,  or  7-8 Chaotic; the road has an Intelligence of 3d6, and there’s a 1-2 in 6 chance it has properties similar to an intelligent sword (see p. 272 OSE core), (5) the road only appears under certain conditions or at certain times of the year (refer to the Magic Chapter on p. 66),  or (6) other. |


27-table-2.md

| d100   | Result       |
|:-------|:-------------|
| 1-10   | Geologic     |
| 11-20  | Structure    |
| 21-30  | Resource     |
| 31-35  | Dungeon      |
| 36-55  | Another road |
| 56-60  | Water        |
| 61-100 | Settlement   |


27-table-3.md

| d10   | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-3   | Unique material. The road is built of an unusual material.  The  road  is  made  from  (1)  one  of the  materials  above,  but  unique  or  rare  to  the region, (2) iron, (3) bone, (4) graves, (5) glass, (6)  high-tech  material  like  plastic  or  concrete, (7) ceramics, (8) living material, (9-10) other.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| 4-6   | Unique  construction.  The  road  is  built  in an  unusual  manner.  It  is  (1)  elevated,  (2) sunken,  (3)  covered,  (4)  hidden,  (5)  goes underground for a portion, (6) other.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 7     | Magical (benign). The road is enchanted in a manner that is beneficial to those traveling on it. It (1) is safer than normal. Wandering monster chances are reduced by 1d2 while on the road, (2) those on the road are under the effects of a permanent  protection  from  evil  spell,  (3)  food does not spoil or go bad while on the road, (4) travelers on the road move faster than normal: if granted, the normal 50% bonus to movement is increased to 75%, or if not granted travelers have a 25% bonus, (5) travelers on the road do not  incur  exhaustion  for  forced  marching,  (6) healing  is  increased:  roll  twice  for  all  healing spells  and  effects  and  take  the  better  of  two results, (7) all travelers on the road are able to understand any spoken language, or (8) other.                                                                                                                                                                                                                                                                                                           |
| 8     | Magical (malign). The road is enchanted in a manner that is dangerous to those traveling on it. (1) It is more dangerous than normal: those traveling on the road have their chances of wandering monsters increased by 1d2, (2) normal rations spoil after a day on the road and iron rations after 1d4 days, (3) movement is slowed: if a speed bonus would normally be granted for maintained roads it is lost, and if not movement is 50% slower, (4) turning undead is  less  potent:  if  attempting  to  turn  undead within  50’  of  the  road  roll  twice,  taking  the lower result, (5) sleep within 50’ of the road is fitful, and does not count as rest for purposes of memorizing spells or avoiding exhaustion, (6) healing magics are minimized: roll twice when determining damage healed, taking the lower  of  the  two  results,  (7)  creatures  slain on the road are either (1-2 incapable of being raised or brought back to life, short of a wish spell, or 3-6 raised as undead within 1d8 days of their death; they will be 1-2 skeletons, 3-4 zombies, 5 wights, or 6 wraiths), or (8) other. |


28-table-1.md

| d100   | Result                      |
|:-------|:----------------------------|
| 1-10   | Road ends in the chosen hex |
| 11-20  | Road is 1d6 miles long      |
| 21-30  | Road is 1d12 miles long     |
| 31-45  | Road is 1d20 miles long     |
| 46-65  | Road is 3d20 miles long     |
| 66-85  | Road is 5d20 miles long     |
| 86-97  | Road is 2d100 miles long    |
| 98-99  | Road is 5d100 miles long    |
| 100    | Road is 10d100 miles long   |


28-table-2.md

| d100   | Result        |
|:-------|:--------------|
| 1-10   | 1d10 years    |
| 11-60  | 10d10 years   |
| 61-99  | 10d100 years  |
| 100    | 10d1000 years |


28-table-3.md

| d100   | Result                                                                                                                                                                                                                                                                                            |
|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-30   | Little  more  than  a  game  trail.  Carts  and wagons  cannot  use it in  difficult terrain, regardless  of  the  condition  of  the  road  (see p.  49,  OSE  core).  Individuals  must  travel in  single  file  whether  mounted  or  on  foot. Subtract 10 from the roll for length of road. |
| 31-50  | Wider trail. Carts and wagons cannot use it in difficult terrain regardless of the condition of  the  road.  Individuals  can  travel  in  two ranks when on foot. Subtract 5 from the roll for length of road.                                                                                   |
| 51-65  | Lane.  Carts  can  use  it  in  difficult  terrain, wagons  cannot.  Individuals  can travel in three ranks on foot or two mounted.                                                                                                                                                               |
| 66-81  | Wider  lane.  Carts  and  wagons  can  use  it in difficult terrain, individuals can travel in four ranks on foot or two mounted.                                                                                                                                                                 |
| 82-92  | Road. Wide enough for two wagons to pass. +5 to the roll for length of road.                                                                                                                                                                                                                      |
| 93-97  | Wide  Road.  Wide  enough  for  four  wagons to pass. +10 to the roll for length of road.                                                                                                                                                                                                         |
| 98-00  | Grand Road. Six  or  more  wagons  can  pass each other. +15 to the roll for length of road.                                                                                                                                                                                                      |


29-table-1.md

| d100   | Result   |
|:-------|:---------|
| 01-05  | Aqueduct |
| 06-40  | Bridge   |
| 41-45  | Canal    |
| 46-55  | Fountain |
| 56-65  | Pond     |
| 66-00  | Well     |


29-table-2.md

| d100   | Result         |
|:-------|:---------------|
| 1-10   | 3d6 feet tall  |
| 11-50  | 4d8 feet tall  |
| 51-90  | 5d10 feet tall |
| 91-100 | 6d20 feet tall |


29-table-3.md

| d100   | Result      |
|:-------|:------------|
| 1-10   | 3d6 feet    |
| 11-40  | 4d10 feet   |
| 41-75  | 5d20 feet   |
| 76-99  | 10d100 feet |
| 100    | 1d4 miles   |


29-table-4.md

| d100   | Result         |
|:-------|:---------------|
| 1-30   | 3d4 feet wide. |
| 31-90  | 5d6 feet wide. |
| 91-100 | 6d8 feet wide. |


29-table-5.md

| d100   | Result                                                                       |
|:-------|:-----------------------------------------------------------------------------|
| 1      | 5d20 feet long (perhaps this is all that remains of a once elaborate system) |
| 2-5    | 10d100 feet long                                                             |
| 6-50   | 1d4 miles long                                                               |
| 51-75  | 3d6 miles long                                                               |
| 76-99  | 5d20 miles long                                                              |
| 100    | 10d100 miles long                                                            |


29-table-6.md

| d100   | Result                                                                    |
|:-------|:--------------------------------------------------------------------------|
| 1-5    | Channel created by hollow logs.                                           |
| 6-30   | Brick. Laid and mortared bricks.                                          |
| 31-65  | Clay.                                                                     |
| 66-90  | Stone.                                                                    |
| 91-99  | Metal. Lead, most likely.                                                 |
| 100    | Exotic Materials. Hollow bones, blown glass, magically shaped stone, etc. |


29-table-7.md

| d100   | Result                                                                     |
|:-------|:---------------------------------------------------------------------------|
| 1-10   | Vines or ropes.                                                            |
| 11-30  | Wood. There’s a 1 in 20 chance that the bridge is movable or a drawbridge. |
| 31-60  | Brick. Laid and mortared bricks, potentially plastered.                    |
| 61-90  | Stone.                                                                     |
| 91-94  | Naturally occurring, carved from the landscape by the elements.            |
| 95-97  | Metal. Iron or steel.                                                      |
| 98-99  | Exotic Materials. Hollow bones, blown glass, magically shaped stone, etc.  |
| 100    | Magical.                                                                   |


30-table-1.md

| d100   | Result              |
|:-------|:--------------------|
| 1-5    | 10d20 feet long     |
| 6-30   | 10d100 feet long    |
| 31-50  | 1d4 miles long      |
| 51-75  | 1d12 miles long     |
| 76-97  | 5d20 feet wide/deep |
| 98-100 | 10d100 miles long   |


30-table-2.md

| d100   | Result              |
|:-------|:--------------------|
| 1-10   | 1d4 feet wide/deep  |
| 11-35  | 2d6 feet wide/deep  |
| 36-65  | 3d8 feet wide/deep  |
| 66-90  | 4d10 feet wide/deep |
| 91-100 | 5d12 feet wide/deep |


31-table-1.md

| d100   | Result                                                                                                         |
|:-------|:---------------------------------------------------------------------------------------------------------------|
| 1-5    | Wood.                                                                                                          |
| 6-40   | Brick. Often coated in plaster or adobe.                                                                       |
| 41-95  | Stone. (1-4) fitted and mortared stone or (5-6) carved from stone.                                             |
| 96-99  | Exotic Material. Bone, petrified wood, living trees, etc.                                                      |
| 100    | Magical.  The fountain is fashioned from magical materials such as never-melting ice, an enormous flower, etc. |


31-table-2.md

| d100   | Result        |
|:-------|:--------------|
| 1-15   | 1d4 feet wide |
| 16-50  | 2d4 feet wide |
| 51-85  | 3d4 feet wide |
| 86-100 | 4d4 feet wide |


32-table-1.md

| d100   | Result           |
|:-------|:-----------------|
| 1-15   | 2d10 feet deep   |
| 16-50  | 5d12 feet deep   |
| 51-85  | 10d20 feet deep  |
| 86-99  | 20d100 feet deep |
| 100    | 1d4 miles deep   |


32-table-2.md

| d100   | Result          |
|:-------|:----------------|
| 1-20   | Wood            |
| 21-60  | Brick           |
| 61-90  | Stone           |
| 91-98  | Metal           |
| 99-100 | Exotic material |


32-table-3.md

| d100   | Result                                |
|:-------|:--------------------------------------|
| 1-10   | Dipper that is reached into the well. |
| 11-60  | Bucket on a rope.                     |
| 61-70  | Mechanical screw.                     |
| 71-85  | Mechanical pump and bladder.          |
| 86-99  | Wind turbine.                         |
| 100    | Magical means.                        |


32-table-4.md

| d100   | Result                         |
|:-------|:-------------------------------|
| 1-5    | Camp                           |
| 6-15   | Farm                           |
| 16-17  | Ferry                          |
| 18-20  | Ford                           |
| 21-25  | Hunting Lodge                  |
| 26-30  | Inn                            |
| 31     | Lighthouse                     |
| 32-35  | Logging Camp                   |
| 36-38  | Military Garrison/Supply House |
| 39-48  | Mill                           |
| 49-55  | Mine                           |
| 56     | Monastery                      |
| 57-65  | Orchard                        |
| 66-70  | Other                          |
| 71-75  | Quarry                         |
| 76-85  | Ranch                          |
| 86-95  | Shrine                         |
| 96-100 | Temple                         |


33-table-1.md

| d100   | Result        |
|:-------|:--------------|
| 1-10   | 1d10 years    |
| 11-60  | 10d10 years   |
| 61-99  | 10d100 years  |
| 100    | 10d1000 years |


33-table-2.md

| d100   | Result              |
|:-------|:--------------------|
| 1-10   | Smaller than 1 acre |
| 11-20  | 1d4 acres           |
| 21-50  | 2d6 acres           |
| 51-75  | 3d8 acres           |
| 76-90  | 4d10 acres          |
| 91-95  | 5d12 acres          |
| 96-100 | 6d20 acres          |


33-table-3.md

| d100   | Result                     |
|:-------|:---------------------------|
| 1-25   | 1d8 cp                     |
| 26-75  | 1d8 sp                     |
| 76-99  | 1d8 gp                     |
| 100    | Something other than money |


34-table-1.md

| d100   | Result         |
|:-------|:---------------|
| 1-50   | 1d4 feet deep  |
| 51-90  | 2d4 feet deep  |
| 91-100 | 3d4 feet deep. |


34-table-2.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                        |
|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-31   | Guards. 1d6+1 guards are in the employ of the  inn.  Treat  as  (1-3)  footmen,  light,  (4-5)  footmen,  heavy,  (6-7)  crossbowmen,  or (8) 1st-level fighters. Every 4 guards will be overseen by a sergeant one level higher. Ex. Five  crossbowmen  will  be  overseen  by  a  1st-level fighter, while four 1st-level fighters will be overseen by a 2nd-level fighter. |
| 32-33  | Guild  Hideout.  The  inn  is  in  fact  a  cover for the local thieves’  guild.  Most  of the employees will knowingly work for or be in the employ of the guild. Refer to the Guide to Thieves’ Guilds for more information.                                                                                                                                                |
| 34-36  | Hirelings. Potential employees can be found at  the  inn.  There  will  be  either  (1-4)  1d4 mercenaries or (5-6) 1d2 potential retainers available  for  hire  at  any  given  time.  If  this result comes up more than once increase the number of potential hirelings by 1.                                                                                             |
| 37-38  | Magic-user.  The  inn  has  a  magic-user  on staff.  While  primarily employed  by the innkeeper  the  magic-user  can  be  hired  to cast  spells  for  the  PCs. The  magic-user  will be (1-3) 1st level, (4-5) 2nd level, or (6) 3rd level.  If  this  result  comes  up  twice  increase the NPC’s level by 1.                                                          |
| 39     | Magical  item.  There  is  one  magical  item available for sale or trade (in exchange for a service). This will be (1-4) a potion or scroll, or (5-6) a permanent item.                                                                                                                                                                                                      |
| 40-49  | Market. The inn serves as the urban center for nearby residents and has a Market Class of 1. Each time this result comes up add 1 to the Market Class.                                                                                                                                                                                                                        |
| 50-57  | Smithy.  The  smithy  will  be  run  by  a  (1-5)  blacksmith  or  (6)  armorer.  If  this  result comes  up  more than  once assume the additional workers are assistants.                                                                                                                                                                                                   |


35-table-1.md

| d100   | Result                                                                                                                                                                                                                                                                                          |
|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 58-59  | Spy. One of the workers at the inn is a spy, sponsored by (1-2) the nearby domain ruler, (3-4)  a  foreign  domain  ruler,  (5)  a  band  of brigands, or (6) other.                                                                                                                            |
| 60-72  | Stables. The inn maintains enclosed stables and stablehands that care for the mounts of travelers. There’s a 1-3 in 6 chance there will be  1d4  randomly  determined  mounts  for sale, and a 1 in 6 chance there is a (1-4) cart or (5-6) wagon for sale.                                     |
| 73-77  | Temple.  The  inn  maintains  a  small  temple that is overseen by a (1-3) 1st-level cleric, (4-5) 2nd-level cleric, or (6) 3rd-level cleric. If this  result  occurs  more  than  once  increase the level of the cleric by 1.                                                                 |
| 78-79  | Threat.  A  hidden  threat  lurks  in  the  inn. One  or  more  of  the  staff  may  be  disguised monsters, or the food may have spoiled and will poison the guests, or a fire may break out at  night.  If  this  result  comes  up  more  than once increase the threat level appropriately. |
| 80-100 | Wall.  The inn is  surrounded  by  a (1-3) wood,  (4-5)  brick,  or  (6)  stone  wall  that is  approximately  eight feet tall.  For  each additional result add another defensive feature (arrow slits, moat, tower, etc.).                                                                    |


37-table-1.md

| d100   | Result   |
|:-------|:---------|
| 1-50   | 25%      |
| 51-75  | 50%      |
| 76-95  | 75%      |
| 96-100 | 100%     |


38-table-1.md

| d100         | Result                               |
|:-------------|:-------------------------------------|
| 1-20         | Force fields                         |
| 21-40        | Illusory images/terrain              |
| 41-60        | Magical walls (of fire, stone, etc.) |
| 61-80        | Zones of repulsion                   |
| 81-100 Other |                                      |


38-table-2.md

| d100   | Result       |
|:-------|:-------------|
| 1-40   | 1 subhex     |
| 41-70  | 1d4 subhexes |
| 71-85  | 3d4 subhexes |
| 86-95  | 4d6 subhexes |
| 96-100 | 1d4 hexes    |


38-table-3.md

| d8   | Result                               |
|:-----|:-------------------------------------|
| 1-3  | 1d6 points of damage (no save)       |
| 4-5  | 2d6 points of damage (no save)       |
| 6-7  | 3d6 points of damage (no save)       |
| 8    | Save vs. spells or be disintegrated. |


38-table-4.md

| d100         | Result               |
|:-------------|:---------------------|
| 1-15         | Boggy/marshy terrain |
| 16-30        | Canyons              |
| 31-45        | Cliffs               |
| 46-60        | Impenetrable foliage |
| 61-75        | Rivers               |
| 76-100 Other |                      |


38-table-5.md

| d100          | Result                   |
|:--------------|:-------------------------|
| 1-40          | Traps. Refer to p.       |
| 41-60         | Trenches. Refer to p. 22 |
| 61-80         | Walls. Refer to p. 21    |
| 81-100 Other. |                          |


39-table-1.md

| d100   | Result                                           |
|:-------|:-------------------------------------------------|
| 1-20   | Living creatures                                 |
| 21-40  | Unliving creatures                               |
| 41-46  | Undead                                           |
| 47-52  | Constructs                                       |
| 53-58  | Dragons                                          |
| 59-64  | Animals                                          |
| 65-70  | Elementals                                       |
| 71-76  | Fey                                              |
| 77-82  | Demons (1-3)/Angels (4-6)                        |
| 83-88  | Humans                                           |
| 89-94  | Humanoids                                        |
| 95-00  | Other (lycanthropes, a specific alignment, etc.) |


40-table-1.md

| d20   | Result                  |
|:------|:------------------------|
| 1-3   | Animal, game            |
| 4-6   | Animal, livestock       |
| 7-8   | Mineral, quarried       |
| 9-10  | Mineral, mined          |
| 11-15 | Vegetable, agricultural |
| 16-20 | Vegetable, industrial   |

MULTIPLE
41-table-1.md

|   Unnamed: 0 | Forest                                        | Jungle        | Fresh Water   | Salt Water   | Hills     | Plains    | Desert Badlands   | Mountain   | Swamp     |
|-------------:|:----------------------------------------------|:--------------|:--------------|:-------------|:----------|:----------|:------------------|:-----------|:----------|
|            1 | Deer                                          | Monkey        | Beaver        | Crab         | Deer      | Deer      | Goat              | Goat       | Deer      |
|            2 | Elk                                           | Water buffalo | Otter         | Eel          | Hare      | Zebra     | Hare              | Hare       | Beaver    |
|            3 | Squirrel                                      | Capybara      | Crocodile     | Mussel       | Boar      | Rhino     | Sheep             | Bear       | Otter     |
|            4 | Rabbit                                        | Pig           | Clams         | Dolphin      | Bear      | Giraffe   | Bison             | Bobcat     | Alligator |
|            5 | Boar                                          | Cougar        | Trout         | Whale        | Fox       | Hare      | Auroch            | Fox        | Snake     |
|            6 | Bear                                          | Elephant      | Bass          | Sea lion     | Wolf      | Bison     | Camel             | Wolf       | Turtle    |
|            7 | Fox                                           | Snake         | Gar           | Sharks       | Groundhog | Fox       | Fox               | Squirrel   | Frog      |
|            8 | Wolf                                          | Hippo         | Eel           | Octopus      | Sheep     | Groundhog | Wolf              | Elk        | Crayfish  |
|            9 | Quail                                         | Parrot        | Goose         | Tuna         | Quail     | Grouse    | Pheasant          | Turkey     | Duck      |
|           10 | Turkey                                        | Toucan        | Duck          | Gull         | Pheasant  | Quail     | Grouse            | Quail      | Clams     |
|           11 | Other, by terrain                             |               |               |              |           |           |                   |            |           |
|           12 | Magical creature, add +1d10x10% to base price |               |               |              |           |           |                   |            |           |


41-table-2.md

| d100   | Result                                                  |
|:-------|:--------------------------------------------------------|
| 1-7    | Camel                                                   |
| 8-14   | Chicken                                                 |
| 15-21  | Cow                                                     |
| 22-28  | Dog                                                     |
| 29-35  | Goat                                                    |
| 36-42  | Horse                                                   |
| 43-49  | Llama                                                   |
| 50-56  | Mink                                                    |
| 57-64  | Other                                                   |
| 65-72  | Oxen                                                    |
| 73-79  | Pig                                                     |
| 50-86  | Reindeer                                                |
| 87-93  | Sheep                                                   |
| 94     | Silkworm (worth  3d6×10%  more than base value)         |
| 95-99  | Turkey                                                  |
| 100    | Magical creature (worth 10d10×10% more than base value) |


42-table-1.md

| Unnamed: 0        | Load     | Enc/load   | Base Price   |
|:------------------|:---------|:-----------|:-------------|
| Quarried Minerals | 1 box    | 10,000 cn  | 150 gp       |
| Stone             | 1 pallet | 5,000 cn   | 1,000 gp     |


42-table-2.md

| d100   | Result                   |
|:-------|:-------------------------|
| 1-20   | Above ground and visible |
| 21-40  | 1d4×5 feet underground   |
| 41-60  | 1d4×10 feet undergound   |
| 61-80  | 2d8×20 feet underground  |
| 81-100 | 3d10×50 feet underground |


42-table-3.md

| d100   | Result            |
|:-------|:------------------|
| 1-7    | Chalk             |
| 8-14   | Clay              |
| 15-21  | Coal              |
| 22-28  | Coquina           |
| 29-35  | Diabas/Gabbro     |
| 36-42  | Granite           |
| 43-49  | Gypsum            |
| 50-56  | Limestone         |
| 57-63  | Marble            |
| 64-78  | Other             |
| 79-84  | Sandstone         |
| 85-91  | Sand              |
| 92-98  | Slate             |
| 99-00  | Special (magical) |


43-table-1.md

| Substance   | Multiplier   |
|:------------|:-------------|
| Copper      | x2           |
| Iron        | x2.5         |
| Lead        | x1.1         |
| Mica        | x1.5         |
| Natron      | x1.5         |
| Pyrite      | x1.2         |
| Silver      | x1.5         |
| Sulfur      | x2           |
| Tin         | x2.25        |
| Zinc        | x2.25        |


43-table-2.md

| d100   | Result                                                             |
|:-------|:-------------------------------------------------------------------|
| 1-4    | Antimony                                                           |
| 5-8    | Arsenic                                                            |
| 9-14   | Copper                                                             |
| 15-18  | Gold                                                               |
| 19-25  | Iron                                                               |
| 26-30  | Lead                                                               |
| 31-34  | Mercury                                                            |
| 35-40  | Mica                                                               |
| 41-46  | Natron                                                             |
| 47-50  | Nickel                                                             |
| 51-54  | Oil                                                                |
| 55-60  | Other                                                              |
| 61-64  | Platinum                                                           |
| 65-70  | Pyrite                                                             |
| 71-75  | Silver                                                             |
| 76-82  | Sulfur                                                             |
| 83-89  | Tin                                                                |
| 90-95  | Zinc                                                               |
| 96-98  | Special (alchemical). Minerals sought after for use by alchemists. |
| 99-100 | Special (magical). Mithril, adamantium, other magical minerals.    |


43-table-3.md

| Substance   | Multiplier   |
|:------------|:-------------|
| Antimony    | x2           |
| Arsenic     | x1.5         |
| Gold        | x1.25        |
| Mercury     | x4           |
| Nickel      | x3           |
| Oil         | x1.1*        |
| Platinum    | x1.1         |


44-table-1.md

| d100   | Result                                                                |
|:-------|:----------------------------------------------------------------------|
| 1-8    | Agate                                                                 |
| 9-14   | Amber                                                                 |
| 15-20  | Amethyst                                                              |
| 21-24  | Aquamarine                                                            |
| 25-27  | Carbuncle                                                             |
| 29-32  | Coral (roll again if not appropriate for location)                    |
| 33     | Diamond                                                               |
| 34-35  | Emerald                                                               |
| 36-41  | Garnet                                                                |
| 42-45  | Jacinth                                                               |
| 46-51  | Jade                                                                  |
| 52-58  | Jasper                                                                |
| 59-65  | Onyx                                                                  |
| 66-68  | Opal                                                                  |
| 69-70  | Other                                                                 |
| 71-74  | Pearl (roll again if not appropriate)                                 |
| 75-82  | Quartz                                                                |
| 83-84  | Ruby                                                                  |
| 85-86  | Sapphire                                                              |
| 87-91  | Topaz                                                                 |
| 92-99  | Turquoise                                                             |
| 100    | Magical  (includes  stones  that  can be used to craft magical items) |


45-table-1.md

| d100   | Result          |
|:-------|:----------------|
| 72-75  | Pepper          |
| 76-79  | Peas            |
| 80-83  | Potato          |
| 84-87  | Spinach         |
| 88-91  | Squash          |
| 92-95  | Turnip          |
| 96-99  | Yam             |
| 100    | Magical/Special |


45-table-2.md

| d100   | Result                                         |
|:-------|:-----------------------------------------------|
| 1-11   | Barley                                         |
| 12-22  | Maize                                          |
| 23-33  | Millet                                         |
| 33-44  | Oats                                           |
| 45-55  | Other                                          |
| 56-66  | Rice                                           |
| 67-77  | Rye                                            |
| 78-88  | Sorghum                                        |
| 89-99  | Wheat                                          |
| 100    | Magical/Special.  Add  1d8×10%  to base price. |


45-table-3.md

| d100   | Result                                                 |
|:-------|:-------------------------------------------------------|
| 1-4    | Apples                                                 |
| 5-8    | Apricots (stone fruit)                                 |
| 9-12   | Avocados                                               |
| 13-16  | Bananas (exotic)                                       |
| 17-20  | Blueberries (berry)                                    |
| 21-24  | Cherry (stone fruit)                                   |
| 25-28  | Grape                                                  |
| 29-32  | Grapefruit (citrus)                                    |
| 33-36  | Kiwi (berry)                                           |
| 37-40  | Lime (citrus)                                          |
| 41-44  | Mandarin (citrus)                                      |
| 45-48  | Mango (exotic)                                         |
| 49-52  | Nectarine (stone fruit)                                |
| 53-56  | Orange (citrus)                                        |
| 57-71  | Other                                                  |
| 72-75  | Passionfruit (berry)                                   |
| 76-79  | Peach (stone fruit)                                    |
| 80-83  | Pear                                                   |
| 84-87  | Plum (stone fruit)                                     |
| 88-91  | Strawberries (berry)                                   |
| 92-95  | Tomato                                                 |
| 96-99  | Watermelon (melon)                                     |
| 100    | Magical/Special.  Add  1d8×10%  to overall base price. |


45-table-4.md

| d100   | Result     |
|:-------|:-----------|
| 1-4    | Artichokes |
| 5-8    | Asparagus  |
| 9-12   | Bamboo     |
| 13-16  | Beans      |
| 17-20  | Beets      |
| 21-24  | Broccoli   |
| 25-28  | Cabbage    |
| 29-32  | Carrots    |
| 33-36  | Cassava    |
| 37-40  | Cucumber   |
| 41-44  | Edamame    |
| 45-48  | Eggplant   |
| 49-52  | Garlic     |
| 53-56  | Gourd      |
| 57-60  | Lettuce    |
| 61-64  | Onions     |
| 65-71  | Other      |


46-table-1.md

| d100          | Result                                      |
|:--------------|:--------------------------------------------|
| 1-4           | Aloe vera                                   |
| 5-8           | Angelica                                    |
| 9-12          | Arnica                                      |
| 13-16         | Belladonna                                  |
| 17-20         | Burdock                                     |
| 21-24         | Cohosh                                      |
| 25-28         | Comfrey                                     |
| 29-32         | Coneflower                                  |
| 33-36         | Dandelion                                   |
| 37-40         | Foxglove                                    |
| 41-44         | Ginseng                                     |
| 45-48         | Hawthorn                                    |
| 49-52         | Horsetail                                   |
| 53-56         | Marshmallow                                 |
| 57-60         | Mushrooms                                   |
| 61-64         | Neem                                        |
| 65-68         | Nettles                                     |
| 69-78         | Other                                       |
| 79-82         | Rosehips                                    |
| 83-86         | Seaweed                                     |
| 87-91         | Snakeroot                                   |
| 92-95 Thistle |                                             |
| 96-99         | Wolfsbane                                   |
| 100           | Magic/Special.  Add  1d8×10% to base price. |


46-table-2.md

| d100        | Result                                         |
|:------------|:-----------------------------------------------|
| 1-4         | Almond                                         |
| 5           | Cardamom                                       |
| 6-9         | Cashew                                         |
| 10-13       | Chestnut                                       |
| 14          | Cacao bean                                     |
| 15          | Clove                                          |
| 16          | Coconut                                        |
| 17          | Coffee                                         |
| 18-20       | Dill                                           |
| 21-24       | Hazelnut                                       |
| 25          | Paprika                                        |
| 26-29       | Pecan                                          |
| 30-31       | Peppercorns                                    |
| 32-33       | Marijuana                                      |
| 3436        | Mint                                           |
| 37-39       | Mushroom, oyster                               |
| 40-41       | Mushroom, shitake                              |
| 42          | Mushroom, psilocybin                           |
| 43-44       | Nutmeg                                         |
| 45-61       | Other                                          |
| 62-65       | Peanut                                         |
| 66-69       | Pecan                                          |
| 70-72       | Pine-nut                                       |
| 73-75       | Pistachio                                      |
| 76-77       | Poppy                                          |
| 78-81       | Oregano                                        |
| 82-84       | Rosemary                                       |
| 85          | Saffron                                        |
| 86-89 Thyme |                                                |
| 90-92       | Tobacco                                        |
| 93-94       | Turmeric                                       |
| 95          | Vanilla                                        |
| 96-99       | Walnut                                         |
| 100         | Magical/Special.  Add  2d6×10%  to base price. |


46-table-3.md

| d100   | Result     |
|:-------|:-----------|
| 1-5    | Bamboo     |
| 6-10   | Birch-bark |
| 11-15  | Cotton     |
| 16-20  | Flax       |


47-table-1.md

| d100   | Result                                            |
|:-------|:--------------------------------------------------|
| 84-87  | Spruce                                            |
| 88-91  | Sycamore                                          |
| 92-95  | Yellow-wood                                       |
| 96-99  | Yew                                               |
| 100    | Magical/Special.  Add  1d8×10%  to the base cost. |


47-table-2.md

| d100   | Result                                                                                                                                  |
|:-------|:----------------------------------------------------------------------------------------------------------------------------------------|
| 21-25  | Grasses (for basketry or similar)                                                                                                       |
| 26-30  | Hemp                                                                                                                                    |
| 31-35  | Jute                                                                                                                                    |
| 36-40  | Other                                                                                                                                   |
| 41-45  | Palm                                                                                                                                    |
| 46-50  | Papyrus                                                                                                                                 |
| 51-55  | Seaweed (reroll if not appropriate)                                                                                                     |
| 56-60  | Sisal                                                                                                                                   |
| 61-65  | Straw                                                                                                                                   |
| 66-99  | Wood  (roll  on  the  (1-4)  Structural or (5-6) Luxury table below, but use the  Wood,  Common  row  on  the Common Trade Goods table) |
| 100    | Magical/Special. Add 5d10×10% to base price.                                                                                            |


47-table-3.md

| d100   | Result                                                                                                                          |
|:-------|:--------------------------------------------------------------------------------------------------------------------------------|
| 1-4    | Bubinga                                                                                                                         |
| 5-8    | Camphor                                                                                                                         |
| 9-12   | Claro Walnut                                                                                                                    |
| 13-16  | Cocobolo                                                                                                                        |
| 17-20  | Ebony                                                                                                                           |
| 21-24  | Elm                                                                                                                             |
| 25-28  | Holly                                                                                                                           |
| 29-32  | Hornbeam                                                                                                                        |
| 33-36  | Koa                                                                                                                             |
| 37-40  | Laurel                                                                                                                          |
| 41-44  | Madrone                                                                                                                         |
| 45-48  | Mahogany                                                                                                                        |
| 49-52  | Mango                                                                                                                           |
| 53-56  | Olive                                                                                                                           |
| 57-68  | Other                                                                                                                           |
| 69-79  | Other  Wood  Species.  Roll  on  the structural  table for  a  wood.  This represents  an  exemplary  specimen of that species. |
| 80-83  | Rosewood                                                                                                                        |
| 84-87  | Sandalwood                                                                                                                      |
| 88-91  | Tamo Ash                                                                                                                        |
| 92-95  | Teak                                                                                                                            |
| 96-99  | Walnut                                                                                                                          |
| 100    | Magical/Special.  Add  1d8×10%  to the overall base cost.                                                                       |


47-table-4.md

| d100   | Result       |
|:-------|:-------------|
| 1-4    | Ash          |
| 5-8    | Alder        |
| 9-12   | Birch        |
| 13-16  | Cedar        |
| 17-20  | Cherry       |
| 21-24  | Chestnut     |
| 25-28  | Cottonwood   |
| 29-32  | Eucalyptus   |
| 33-36  | Fir          |
| 37-40  | Ginkgo       |
| 41-44  | Hickory      |
| 45-48  | Larch        |
| 49-52  | Maple        |
| 53-56  | Oak          |
| 57-67  | Other        |
| 68-71  | Pine, yellow |
| 72-75  | Poplar       |
| 76-79  | Purpleheart  |
| 80-83  | Redwood      |


51-table-1.md

| d100   | Result                                                            |
|:-------|:------------------------------------------------------------------|
| 1-4    | Amber Creeping Vine (OSRIC, p. 269)                               |
| 5-8    | Assassin Vine (S&W Monster Book, p. 6)                            |
| 9-12   | Black Pudding                                                     |
| 13-16  | Brown Mold (OSRIC, p. 297)                                        |
| 17-20  | Falshantog-Yoth “The  Hungering  Vines” (S&W Monster Book, p. 32) |
| 21-24  | Fungal Creeper (S&W Monster Book, p. 34)                          |
| 25-28  | Gas Spore (LL AEC, p.126)                                         |
| 29-32  | Gelatinous Cube                                                   |
| 33-36  | Grey Ooze                                                         |
| 37-40  | Green Slime                                                       |
| 41-44  | Ochre Jelly                                                       |
| 45-64  | Other                                                             |
| 65-68  | Shambling Mound (LL AEC, p. 136)                                  |
| 69-72  | Spiderweed (S&W Monster Book, p. 92)                              |
| 73-76  | Strangleweed (LL AEC, p. 138)                                     |
| 77-80  | Stunjelly (OSRIC, p. 316)                                         |
| 81-84  | Trapper (OSRIC, p. 317)                                           |
| 85-88  | Vampire Tree (S&W Monster Book, p. 103)                           |
| 89-92  | Violet Fungi (LL AEC, p. 126)                                     |
| 93-96  | Yellow Mold                                                       |
| 97-100 | Ygg “Gallows Tree” (S&W Monster Book, p. 109)                     |


53-table-1.md

| d12   | Result   |
|:------|:---------|
| 1-2   | Geologic |
| 3-4   | Resource |
| 5-6   | Terrain  |
| 7-8   | Water    |
| 9-12  | Magic    |


53-table-2.md

| d100                       | Result                                                                                                                                                                                                                                                     |
|:---------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-20                       | Hit point loss. The disease causes (1-3) 1 hp loss  per  interval,  (4-5)  1d4  hp  per  interval, (6) 1d8 hp per interval.                                                                                                                                |
| 21-40                      | Ability score loss. The disease causes a loss of (1-3) 1 point per interval, (4-5) 1d2 points per  interval,  or  (6)  1d4  points  per  interval. Determine the  score  affected  at  random, although the same disease affects all victims the same way. |
| 41-45                      | Ability loss. (such as the ability to cast spells) Use discretion here. There’s a 1-5 in 6 chance a disease with this effect is magical.                                                                                                                   |
| 46-65                      | Movement reduction. The disease causes a reduction  in  the  victim’s  movement  rate  of 10’ per interval.                                                                                                                                                |
| 66-80                      | Penalties to Rolls. Those affected suffer a (1-3) –1 penalty, (4-5) –2 penalty, or (6) –1 per interval penalty to all rolls made.                                                                                                                          |
| 81-94                      | Death. The target dies at the end of the time interval.                                                                                                                                                                                                    |
| 95-98                      | Two of the above.                                                                                                                                                                                                                                          |
| 99-100 Three of the above. |                                                                                                                                                                                                                                                            |


54-table-1.md

| d10   | Result                                                                                                                                                                                                                                                                                                                                                   |
|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-2   | Asphyxiation.  There  is  no  oxygen  present in the cloud.  Those  within  will  die  of asphyxiation  within  a  number  of  rounds equal to their Constitution score.                                                                                                                                                                                 |
| 3-4   | Fire. The gas is extremely flammable. There’s a 1-2 in 6 chance per round that an open flame is present that it bursts like a fireball, doing (1-3)  3d6  points  of  damage,  (4-5)  6d6  points  of damage, or (6) 9d6 points of damage to everyone within  range  unless  they  succeed  on  a  Save  v. Breath (in which case half damage is taken). |
| 5-6   | Nausea. All within the gas cloud must Save v.  Poison  or  be  affected  with  a  nausea  like that caused by centipede poison, but lasting only 1d4 turns after leaving the cloud.                                                                                                                                                                      |
| 7-8   | Has an effect other than those listed.                                                                                                                                                                                                                                                                                                                   |
| 9-10  | Sleep.  All  within  the  cloud  must  Save  v. Poison or fall asleep for (1-3) 1d10 turns, (4-5) 1d12 hours, or (6) until removed from the cloud of gas.                                                                                                                                                                                                |


55-table-1.md

| d10   | Result        |
|:------|:--------------|
| 1-2   | 1d4 turns old |
| 3-4   | 1d4 hours old |
| 5-6   | 3d8 hours old |
| 7-8   | 1d4 days old  |
| 9-10  | 1d8 days old  |


56-table-1.md

| d10   | Result                       |
|:------|:-----------------------------|
| 1-40  | 1st-level dungeon            |
| 41-69 | 2nd-level dungeon            |
| 70-83 | 3rd-level dungeon            |
| 84-93 | 4th-5th-level dungeon        |
| 94-97 | 6th-7th-level dungeon        |
| 98-99 | 8th-9th-level dungeon        |
| 100   | 10th-level or higher dungeon |


57-table-1.md

| d10    | Result   |
|:-------|:---------|
| 1-15   | 1d4+1    |
| 16-30  | 2d4      |
| 31-45  | 3d6      |
| 46-60  | 4d8      |
| 61-75  | 5d10     |
| 75-85  | 6d12     |
| 86-95  | 7d20     |
| 96-100 | 8d100    |


58-table-1.md

| d100   | Result         |
|:-------|:---------------|
| 1-25   | 1 subhex       |
| 26-50  | 1d4+1 subhexes |
| 51-75  | 3d4 subhexes   |
| 76-85  | 4d8-1 subhexes |
| 86-95  | 1 hex          |
| 96-98  | 1d6 hexes      |
| 99-100 | 2d6 hexes      |


59-table-1.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-10   | Glacier. A mass of densely packed, slowly moving snow. Those on the glacier have their movement reduced by 1/2, suffer the same risk of sun-blindness as on a salt flat, and have a 1 in 6 chance of encountering a hazard for each subhex they enter on the glacier (most likely a crevasse or a sinkhole).                                                                                                                                                                                                                                                                                           |
| 10-20  | Hot Springs. See p. in the section on water features.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| 21-30  | Landlocked sand dunes. All that remains of an ancient, land-locked sea or ocean. Treat as desert.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 31-40  | Mudflats. A stretch of barren clay that cracks when it dries. When wet, it becomes slick and difficult to traverse. Reduce movement by 1/2 when traveling through a wet mudflat.                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 41-50  | Other.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| 51-60  | Petrified Forest. The remains of an ancient forest can be found here, the trees turned to stone. There’s only a 1 in 6 chance the trees are actually standing, otherwise they are lying on the ground.                                                                                                                                                                                                                                                                                                                                                                                                 |
| 61-70  | Rock Formations. Unusual rock formations dot the landscape: towers of stone such as the Devil’s Tower in Wyoming or the Stone Forest in China, or unusual boulder deposits (see Geological features for more information).                                                                                                                                                                                                                                                                                                                                                                             |
| 71-80  | Salt flat. Risk of sun blindness. For every day spent on the flats without eye protection make a save versus wands. Failure indicates the creature is partially blinded, suffering a –2 penalty to all rolls. The blindness disappears in 1d4 days after leaving.                                                                                                                                                                                                                                                                                                                                      |
| 81-90  | Temperate Rain Forest. Due to unique weather patterns the forest receives a large amount of rain. Often features larger-than-normal trees, moss, mushrooms, etc.                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 91-95  | Volcano. The volcano will be (1-7) not currently active but will erupt in 1d100 months, (8-14) not currently active but will erupt in 1d100 years, (15-19) extinct, (20) currently erupting (treat as hazard).                                                                                                                                                                                                                                                                                                                                                                                         |
| 96-99  | Out of place. The feature is out of place but still mundane (although it may have been created by magical means!): a mountain in the middle of a prairie, or a land-locked sea in hill country.                                                                                                                                                                                                                                                                                                                                                                                                        |
| 100    | Magical/magically  created  terrain. This  category  includes  things  like  fungal  forests, fields of flowers that magically put those walking through them to sleep, areas where gravity  is  increased  or  decreased,  etc. The  terrain  itself  could  have  a  magical  effect  – for instance, it could be a null-magic zone, where no magic functions – or it could be obviously magically created, such as an entire hex where the ground has been turned into bright green glass. Regardless, the terrain type here is both clearly out of place and clearly artificial/magical in nature. |

MULTIPLE
60-table-1.md

| 1d6   | 1                 | 2          | 3               | 4        | 5                           | 6                   |
|:------|:------------------|:-----------|:----------------|:---------|:----------------------------|:--------------------|
| 1d8   | Forest            | Flat       | Arid            | Wetlands | Mountains                   | Hills               |
| 1     | Light, Coniferous | Prairie    | Desert, Cold    | Bog      | Muntains, Small-Barren      | Hills, Grasslands   |
| 2     | Heavy, Coniferous | Grazing    | Desert, Hot     | Marsh    | Mountains, Small-Forested   | Hills, Barren       |
| 3     | Light, Deciduous  | Farmland   | Desert, Coastal | Swamp    | Mountains, Tall-Barren      | Hills, Forested     |
| 4     | Heavy, Deciduous  | Shrublands | Desert, Rocky   | Jungle   | Mountains, Tall-Forested    | Hills, Shrub        |
| 5     | Light, Mixed      | Savanna    | Badlands        | River    | Mountains, Tall-Snow Capped | Hills, Jungle       |
| 6     | Heavy Mixed       | Flats      | Steppes         | Moor     | Volcano                     | Hills, Transitional |
| 7     | Rainforest        | Tundra     | Flats           | Fungal   | Plateau                     | Hills, Lone         |
| 8     | Other             | Other      | Other           | Other    | Other                       | Other               |


62-table-1.md

| Table 3                | Unnamed: 1      |
|:-----------------------|:----------------|
| d100                   | Result          |
| 1-15                   | Class 5 Market  |
| 16-45                  | Class 6 Market  |
| 46-65                  | Class 7 Market  |
| 66-86                  | Class 8 Market  |
| 86-98                  | Class 9 Market. |
| 99-100 Class 10 Market |                 |


62-table-2.md

| d100         | Result      |
|:-------------|:------------|
| 1-50         | Humans      |
| 51-75        | Demi-Humans |
| 76-90        | Humanoids   |
| 91-100 Other |             |


62-table-3.md

| Table 1   | Unnamed: 1     |
|:----------|:---------------|
| d100      | Result         |
| 1-50      | Class 1 Market |
| 51-90     | Class 2 Market |
| 91-99     | Class 3 Market |
| 100       | Class 4 Market |


62-table-4.md

| Table 2   | Unnamed: 1     |
|:----------|:---------------|
| d100      | Result         |
| 1-25      | Class 1 Market |
| 26-45     | Class 2 Market |
| 46-60     | Class 3 Market |
| 61-75     | Class 4 Market |
| 76-90     | Class 5 Market |
| 91-99     | Class 6 Market |
| 100       | Class 7 Market |


63-table-1.md

| d100   | Result   |
|:-------|:---------|
| 1-35   | Brook    |
| 36-60  | Creek    |
| 61-85  | Stream   |
| 86-100 | River    |


64-table-1.md

| d100   | Result            |
|:-------|:------------------|
| 1-50   | 4d10 feet wide    |
| 51-75  | 10d20 feet wide   |
| 76-90  | 10d100 feet wide  |
| 91-100 | 10d100 yards wide |


64-table-2.md

| d100   | Result             |
|:-------|:-------------------|
| 1-10   | 1d4 weeks prior    |
| 11-20  | 1d12 months prior  |
| 21-80  | 1d10 years prior   |
| 81-90  | 2d100 years prior  |
| 91-100 | 10d100 years prior |


65-table-1.md

| d100   | Result           |
|:-------|:-----------------|
| 1-25   | 1d100 feet long  |
| 26-50  | 10d100 feet long |
| 51-75  | 1d4 miles long   |
| 76-100 | 1d8 miles long   |


66-table-1.md

| d100   | Result           |
|:-------|:-----------------|
| 1-40   | 1d10 feet high   |
| 41-75  | 2d20 feet high   |
| 76-90  | 3d100 feet high  |
| 91-99  | 10d100 feet high |
| 100    | 20d100 feet high |


66-table-2.md

| d100   | Result                                       |
|:-------|:---------------------------------------------|
| 1-15   | 10d100 yards in diameter and 3d4 feet deep.  |
| 15-55  | 1d4 miles in diameter and 3d6 feet deep.     |
| 56-75  | 2d6 miles in diameter and 4d6 feet deep.     |
| 76-90  | 3d12 miles in diameter and 5d6 feet deep.    |
| 91-98  | 5d20 miles in diameter and 5d10 feet deep.   |
| 99-100 | 10d100 miles in diameter and 5d20 feet deep. |

^232946


66-table-3.md

| d100   | Result                                                                  |
|:-------|:------------------------------------------------------------------------|
| 1-20   | Less than a mile wide. Smaller bays are referred to as coves or inlets. |
| 21-40  | 1d4 miles wide                                                          |
| 40-55  | 2d6 miles wide                                                          |
| 56-70  | 3d8 miles wide                                                          |
| 71-85  | 4d10 miles wide                                                         |
| 86-100 | 5d20 miles wide                                                         |


67-table-1.md

| d100   | Result                                                |
|:-------|:------------------------------------------------------|
| 1-10   | 10d100 feet wide/1d4 miles long/5d20 feet deep        |
| 11-50  | 10d100  yards  wide/2d6  miles long/10d20 feet deep   |
| 51-90  | 1d4 miles wide/3d8 miles long/5d100 feet deep         |
| 91-100 | 1d6+1  miles  wide/4d10  miles  long/10d100 feet deep |


67-table-2.md

| d100   | Result           |
|:-------|:-----------------|
| 1-10   | 1d4 miles wide   |
| 11-30  | 2d6 miles wide   |
| 31-50  | 3d8 miles wide   |
| 51-75  | 4d10 miles wide  |
| 76-95  | 5d20 miles wide  |
| 96-100 | 6d100 miles wide |


67-table-3.md

| d100   | Result              |
|:-------|:--------------------|
| 1-10   | 1d4 weeks prior.    |
| 11-20  | 1d12 months prior.  |
| 21-80  | 1d10 years prior.   |
| 81-90  | 2d100 years prior.  |
| 91-100 | 10d100 years prior. |


67-table-4.md

| d100   | Result                   |
|:-------|:-------------------------|
| 1-10   | 5d20 miles/10d20 feet    |
| 11-50  | 10d20 miles/5d100 feet   |
| 51-90  | 5d100 miles/10d100 feet  |
| 91-100 | 10d100 miles/20d100 feet |


69-table-1.md

| Table 11.2 – Magical Effects   | Unnamed: 1              |
|:-------------------------------|:------------------------|
| d100                           | Result                  |
| 1-15                           | Climate                 |
| 16-30                          | Flora and Fauna         |
| 31-55                          | Other                   |
| 56-70                          | Ley Lines               |
| 71-85                          | Resonance or Dissonance |
| 86-100                         | Space and Time          |


69-table-2.md

| d100   | Result         |
|:-------|:---------------|
| 1-25   | 1 subhex       |
| 26-50  | 1d4+1 subhexes |
| 51-75  | 3d4 subhexes   |
| 76-85  | 4d8–1 subhexes |
| 86-95  | 1 hex          |
| 96-98  | 1d6 hexes      |
| 99-100 | 2d6 hexes      |


7-table-1.md

| d20   | Result     |
|:------|:-----------|
| 1-4   | Geologic   |
| 5-8   | Structure  |
| 9-12  | Resource   |
| 13    | Hazard     |
| 14    | Sign       |
| 15    | Dungeon    |
| 16-17 | Terrain    |
| 18    | Settlement |
| 19    | Water      |
| 20    | Magic      |


7-table-2.md

| d20   | Result                   |
|:------|:-------------------------|
| 1-3   | Geologic                 |
| 4-6   | Structure                |
| 7-9   | Resource                 |
| 10-12 | Lair                     |
| 13    | Hazard (1-3), Sign (4-6) |
| 14    | Dungeon                  |
| 15    | Terrain                  |
| 16    | Settlement               |
| 17    | Water                    |
| 18    | Magic                    |
| 19-20 | No Feature               |


70-table-1.md

| d100   | Result          |
|:-------|:----------------|
| 41-60  | Grasses/Flowers |
| 61-80  | Shrubs          |
| 81-100 | Trees           |


70-table-2.md

| d100         | Result                            |
|:-------------|:----------------------------------|
| 1-16         | (1-3) Beneficial or (4-6) Baneful |
| 17-32 Mobile |                                   |
| 33-48        | Sentient                          |
| 49-64        | Unusual Size                      |
| 65-82        | Unusual Form                      |
| 81-92        | Unusual Features                  |
| 97-99        | Roll Twice                        |
| 100          | Roll Thrice                       |


70-table-3.md

| d100                          | Result           |
|:------------------------------|:-----------------|
| 1-30                          | Plants           |
| 31-60                         | Animals          |
| 61-90                         | Other Creatures  |
| 91-98                         | Two of the above |
| 99-100 All three of the above |                  |


70-table-4.md

| d100                  | Result                                                                                        |
|:----------------------|:----------------------------------------------------------------------------------------------|
| 1-10                  | All of the plant-life in the area                                                             |
| 11-40                 | A specific species of plant-life                                                              |
| 41-70                 | A small number of particular plants within  the  area:  (1-3)  1d20,  (4-5) 5d20, (6) 10d100. |
| 71-100 A single plant |                                                                                               |


70-table-5.md

| d100   | Result      |
|:-------|:------------|
| 1-20   | Moss/Lichen |
| 21-40  | Fungi       |


71-table-1.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-40   | Plants  survive  on  something  other than sunlight:  (1-2)  meat,  (3)  heat  or  cold,  (4) esoterica (thoughts, emotions, etc.), (5) ore (gold, copper, etc.), or (6) magic.                                                                                                                                                                                                                                                                                                                                                       |
| 41-80  | Plants  produce  unusual  fruit:  (1)  made  of  a valuable material (gold, spun glass), (2) with healing (1-3) or harmful (4-6) properties, (3) containing  a  magical  spell  that  is  triggered by eating,  or  breaking,  or throwing, (4) which  transports  the  eater  to  another  plane or  dimension,  (5)  which  acts  as  a  randomly determined potion, or (6) that when thrown will turn into a randomly determined monster. The plant produces (1-3) only a single special fruit, (4-5) 1d10 fruit, (6) 1d100 fruit. |
| 81-100 | Roll on Table 11.2 for an additional effect.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |


71-table-2.md

| d100   | Result    |
|:-------|:----------|
| 1-10   | 25%       |
| 11-30  | 50%       |
| 31-50  | 75%       |
| 51-90  | 100%      |
| 91-100 | 3d6 times |


71-table-3.md

| d100                   | Result                                                                             |
|:-----------------------|:-----------------------------------------------------------------------------------|
| 1-10                   | All of the animals in the area                                                     |
| 11-40                  | A specific species of animal                                                       |
| 41-70                  | A  small  number  of  animals  within the area: (1-3) 1d20, (4-5) 5d20, (6) 10d100 |
| 71-100 A single animal |                                                                                    |


71-table-4.md

| d100   | Result                                                                                    |
|:-------|:------------------------------------------------------------------------------------------|
| 1-25   | Different color (1-3) bark, (4-6) leaves, (7-8) both.                                     |
| 26-50  | Different shape.  Perhaps the trunk and branches are geometric.                           |
| 51-75  | Different texture/surface.                                                                |
| 76-100 | Non-native  plants.  Instead  of  trees,  maybe they are giant mushrooms, or waving kelp. |


71-table-5.md

| d100           | Result     |
|:---------------|:-----------|
| 1-20           | Insects    |
| 21-40          | Amphibians |
| 41-60          | Reptiles   |
| 61-80          | Bird       |
| 81-100 Mammals |            |


72-table-1.md

| d100   | Result                            |
|:-------|:----------------------------------|
| 1-16   | (1-3) Beneficial or (4-6) Baneful |
| 17-32  | Awakened                          |
| 33-48  | Sentient                          |
| 49-64  | Unusual Size                      |
| 65-82  | Unusual Form                      |
| 81-92  | Unusual Features                  |
| 97-99  | Roll Twice                        |
| 100    | Roll Thrice                       |


72-table-2.md

| d100   | Result    |
|:-------|:----------|
| 1-10   | 25%       |
| 11-30  | 50%       |
| 31-50  | 75%       |
| 51-90  | 100%      |
| 91-100 | 3d6 times |


73-table-1.md

| d100   | Result                                                                                                                                                                                                                                 |
|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-25   | Different (1-3) skin/fur, (4-6) color, (7-8) both.                                                                                                                                                                                     |
| 26-50  | Different  shape.  The  animal  may  have  six legs instead of four, or wings (and potentially a fly speed) where it had none before.                                                                                                  |
| 51-75  | The animal is a mixture of (1-3) two, (4-5) three, or  (6)  four  animals,  sharing  characteristics of  all  of  them.  There’s  a  1  in  6  chance  per animal type that the main characteristic is a hindrance, or non-beneficial. |
| 76-100 | Non-native  animals. In this  part  of the world perhaps fish swim through the air as if it were water, or penguins hunt the plains for insects.                                                                                       |


73-table-2.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 71-85  | Special Defense. The animal gains a special defense.  This  is  (1)  resistance  to  a  form  of damage (bludgeoning, fire, etc.), (2) immunity to a form of damage, (3) regeneration (1-3: 1 hp per round, 4-5: 2 hp per round, or 6: 3 hp per round), (4) successful attacks upon them damage or negate weapons (such as a living iron  statue’s  ability  to  absorb  weapons),  (5) some of the damage suffered from attacks is borne by the attacker, or (6) the creature can change  form  to  escape  (such  as  a  vampire’s ability to turn into a bat or mist). |
| 86-90  | Magical Manifestation. The animal can cast a randomly determined spell of level (1-3) 1, (4-5) 2, or (6) 3. This spell is used as a special ability  and  can  be  used  (1-4)  once  per  day, (5-7) twice per day, (8-9) three times per day, or (10) is always active/available.                                                                                                                                                                                                                                                                                       |
| 91-97  | Movement. The  creature’s  Move  score (1-4) increases  by  (1-3)  10’,  (4-5)  20’,  or  (6)  30’,  or (5-6)  they  gain  a  new  form  of  movement  in addition to their old form. This new form is (1-2) 1 category slower than their current form, (3-4) the same speed, or (5-6) 1 category faster.                                                                                                                                                                                                                                                                 |
| 98-99  | Roll Twice.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| 100    | Roll Thrice.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |


73-table-3.md

| d100   | Result                                                                                                                                                                                                                                                                                                                         |
|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-15   | Additional  hit  points.  They  have  (1-3)  +1, (4-5) +2, or (6) +4 hit points.                                                                                                                                                                                                                                               |
| 16-20  | Additional Hit Dice. The creatures’ Hit Dice (1-4) increases by (1-3) 1, (4-5) 2, or (6) 3, or (5-6) increases from 1d8 to (1-4) 1d10 or (5-6) 1d12.                                                                                                                                                                           |
| 21-35  | Armor Class. The creatures’ AC improves by (1-3) 1, (4-5) 2, or (6) 3.                                                                                                                                                                                                                                                         |
| 36-50  | Damage. The creature’s existing damage (1-4) increases by one die type (from d6 to d8, for instance) or (5-6) they gain an additional attack  at  a  die  type  one  lower  than  their current lowest attack (if the animal can attack twice doing 1d6 points of damage they gain a third attack doing 1d4 points of damage). |
| 51-55  | Saving Throws. The animal uses the Fighter Saving Throw chart at the normal progression (Animal HD equals fighter level, as opposed to half progression).                                                                                                                                                                      |
| 56-70  | Special  Attack.  The  animal  gains  a  special attack.  This  is  (1)  poison,  (2)  disease,  (3) elemental, (4)  paralyzing, (5) a special combat maneuver (grapple, trample, etc.), or (6) something else.                                                                                                                |


73-table-4.md

| d100   | Result                                                                                                                                                                                                                                                                                                |
|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-40   | Animals feed  on  something  other than their  normal  diet:  (1-2)  meat instead  of vegetation,  or  vice  versa,  (3)  heat  or  cold, (4) esoterica (thoughts, emotions, etc.), (5) ore (gold, copper, etc.), or (6) magic.                                                                       |
| 41-80  | Parts of the animal are valuable for use by alchemists  or  magicians.  There’s  a  1  in  6 chance  that  the  body  part  can  actually  be used  by  the  animal  for  offense  or  defense (a  gland  that  allows  them  to  breath  fire, for instance),  but  otherwise it is  non-functional. |
| 81-100 | Roll on Table 11.2 for an additional effect.                                                                                                                                                                                                                                                          |


74-table-1.md

| d100   | Result                                                                           |
|:------ |:-------------------------------------------------------------------------------- |
| 1-10   | All of the creatures in the area                                                 |
| 11-40  | A specific species                                                               |
| 41-70  | A small number of creatures within the area: (1-3) 1d20, (4-5) 5d20, (6) 10d100. |
| 71-100 | A single creature                                                                |


74-table-2.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 61-80  | Plane-touched. The creature (1-4) possesses  an  ancestry that  comes from another plane or dimension or (5-6) actually is  from  another  dimension  or  plane.  They may exhibit traits from that plane, such as a creature with an ancestry tracing back to the plane of Fire being immune to fire, or similar,  or  may  actually  exist  out  of  sync with the normal world.                                                                                                                 |
| 81-100 | Spellcaster. The creature(s) possess a native ability  to  cast  spells.  They  do  so  as  a  (1-2)  magic-user,  (3-4)  cleric,  (5)  druid,  (6) illusionist, or (7-8) other spellcasting class. They  do  so  either  (1-4)  at  a  class  level,  if they belong to the given class, meaning that not all creatures in the area can cast spells, or  (5-6)  innately,  with  all  members  of  the species in the area casting spells as a caster of level (1-3) 1d4, (4-5) 1d8, or (6) 1d12. |


74-table-3.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                             |
|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-20   | Alternate Mode of Communication. The creature communicates via (1-4) empathy (projecting their emotions) or (5-6) telepathy (projecting their thoughts). There’s a 1 in 6 chance that a creature that can  do  this  can  also  read  emotions  and thoughts  in  others,  and  a  further  1  in  6 chance  that  this  is  their  only  means  of communication. |
| 21-40  | Immortality.  The creature is immortal and (1-3) cannot die of old age but can die of  disease  or  injury,  (4-5)  can  only  die  of injury, or (6) cannot be permanently slain.                                                                                                                                                                                 |
| 41-60  | Out of Time. The creature is from the (1-2)  past,  (3-4)  future,  or  (5-6)  an  alternate version  of  reality.  There’s  a  1  in  6  chance that whatever magic has brought them here can  fling  the  unwary  to  (1-4)  their  native time or (5-6) a random time.                                                                                          |


74-table-4.md

| d100   | Result                                                                                                                                                                                                                                                             |
|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-15   | Beneficial/Baneful to those  of  different alignments. Refer to the examples above in Flora/Fauna.                                                                                                                                                                 |
| 16-30  | Helpful  to  those  of  the  same  alignment. Creatures of the same alignment as the land enjoy (1) a +1 bonus to AC, (2) +1 to attack rolls,  (3)  +1  to  damage  rolls,  (4)  +1  to  all Saves,  (5)  regenerate  1  hp  per  turn,  or  (6) two of the above. |


75-table-1.md

| d100   | Result                                                                                                                                                                                                                                                                                              |
|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 31-45  | Dangerous to those of a different alignment. Creatures of a different alignment suffer a (1) penalty of 1 to AC, (2) –1 penalty to attack rolls, (3) –1 penalty to damage rolls, (4) –1 penalty to Saves, (5) will not heal naturally in the region, or (6) two of the above.                       |
| 46-60  | Dampens  spells.  Spells  with  an  opposite alignment descriptor do not function within the  area.  Inside  a  Chaotically  aligned  area the spells detect evil and protection from evil would not function.                                                                                      |
| 61-75  | Inimical to those of an opposite alignment. There’s  a  1-2 in  6  chance  that in  order to enter the region those  of  differing alignments must make a Save v. Spells. The roll is penalized by 1d4 if the difference is greater  than  one  step  (Lawful  characters entering a Chaotic land). |
| 76-90  | Unease. Those not of the alignment of the land are uneasy, suffering (1-3) a –1 penalty to surprise rolls, (4-5) the inability to rest, or (6) both.                                                                                                                                                |
| 91-96  | Roll Twice. Redundant results are cumulative.                                                                                                                                                                                                                                                       |
| 97-100 | Roll  Thrice. Redundant results are cumulative.                                                                                                                                                                                                                                                     |


75-table-2.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                |
|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-25   | The  residents  are  all  magically inclined. Most  are  equivalent to  1st-level  magic-users.                                                                                                                                                                                                                                       |
| 26-50  | The  settlement  has  some  form  of  magical or  unusual  defense:  (1) trained  griffons or  similar,  (2)  golems  guarding  the  gates, (3)  wards  that  prevent  entry  by  invisible creatures,  (4)  fixed  crossbows  that  shoot bolts of fire, (5) walls magically reinforced to have extra hit points, or (6) roll twice. |
| 51-70  | The settlement is airborne. It is built (1) on a  cloud,  (2)  on  a  floating  rock,  (3)  on  the back  of  an  enormous  flying  creature,  (4) suspended between two mountains.                                                                                                                                                   |
| 71-90  | The  settlement  is  mobile.  It  (1)  is  built  on the back  of an enormous creature, (2) has legs and walks around like a spider, (3) has wheels and a sail, (4) floats on water.                                                                                                                                                  |
| 91-100 | Other.                                                                                                                                                                                                                                                                                                                                |


76-table-1.md

|   d100 | Result                                                                             |
|-------:|:-----------------------------------------------------------------------------------|
|      1 | Acid Fog (6th-level illusionist)                                                   |
|      2 | Animate  Dead  (dead  are  animated  within 1d4 rounds of death, 5th-level MU)     |
|      3 | Auditory Illusion (1st-level illusionist)                                          |
|      4 | Blacklight (3rd-level illusionist)                                                 |
|      5 | Bless/Blight (2nd-level cleric)                                                    |
|      6 | Blur (2nd-level illusionist)                                                       |
|      7 | Chaos (5th-level illusionist)                                                      |
|      8 | Cloudkill (5th-level MU)                                                           |
|      9 | Confusion (4th-level MU)                                                           |
|     10 | Dancing Lights (1st-level illusionist)                                             |
|     11 | Demi-shadow Monsters (5th-level illusionist)                                       |
|     12 | Detect Evil (1st-level cleric, 2nd-level MU)                                       |
|     13 | Dispel Illusion (3rd-level illusionist)                                            |
|     14 | Detect Invisible (2nd-level MU)                                                    |
|     15 | Dispel Magic (3rd-level MU)                                                        |
|     16 | Dream Quest (6th-level illusionist)                                                |
|     17 | Emotion (4th-level illusionist)                                                    |
|     18 | Entangle (1st-level druid)                                                         |
|     19 | ESP  (2nd-level  MU,  all  who  enter  the  area can sense the thoughts of others) |
|     20 | Faerie Fire (1st-level druid)                                                      |
|     21 | False Aura (2nd-level illusionist)                                                 |
|     22 | Fascinate  (centered  on  a  feature  within  the area, 2nd-level illusionist)     |
|     23 | Fear (3rd-level illusionist)                                                       |
|     24 | Feeblemind (5th-level MU)                                                          |
|     25 | Illusion (5th-level illusionist)                                                   |
|     26 | Impersonation (6th-level illusionist)                                              |
|     27 | Growth of Nature (3rd-level druid)                                                 |
|     28 | Hallucinatory  Terrain  (4th-level  MU,  3rd-level illusionist)                    |
|     29 | Haste (3rd-level MU)                                                               |
|     30 | Heat Metal (2nd-level druid)                                                       |


76-table-2.md

| d100   | Result                                                                                    |
|:-------|:------------------------------------------------------------------------------------------|
| 31     | Hypnotic Pattern (2nd-level illusionist)                                                  |
| 32     | Hypnotism (1st-level illusionist)                                                         |
| 33     | Improved Phantasmal Force (2nd-level illusionist)                                         |
| 34     | Insect Plague (5th-level cleric)                                                          |
| 35     | Invisibility (2nd-level MU)                                                               |
| 36     | Levitate (2nd-level MU)                                                                   |
| 37     | Light/Darkness (1st-level cleric/MU)                                                      |
| 38     | Manifest Dream (6th-level illusionist)                                                    |
| 39     | Massmorph (4th-level MU)                                                                  |
| 40     | Maze of Mirrors (5th-level illusionist)                                                   |
| 41     | Nondetection (3rd-level illusionist)                                                      |
| 42     | Permanent Illusion (6th-level illusionist)                                                |
| 43     | Obscuring Mist (2nd-level druid)                                                          |
| 44-74  | Other                                                                                     |
| 75-76  | Roll two times                                                                            |
| 77     | Roll three times                                                                          |
| 78     | Pass Plant (5th-level druid, only affects certain plants, use Flora section to determine) |
| 79     | Phantasmal Force (1st-level illusionist, 2nd-level MU)                                    |
| 80     | Phantasmal Killer (4th-level illusionist)                                                 |
| 81     | Protection from Evil/Good (1st-level cleric/MU)                                           |
| 82     | Remove Fear/Cause Fear (1st-level cleric)                                                 |
| 83     | Seeming (5th-level illusionist)                                                           |
| 84     | Shades (6th-level illusionist)                                                            |
| 85     | Silence 15’ radius (larger than normal radius, 2nd-level cleric)                          |
| 86     | Shadow Monsters (4th-level illusionist)                                                   |
| 87     | Shadowcast (5th-level illusionist)                                                        |
| 88     | Shadowy Transformation (5th-level illusionist)                                            |
| 89     | Sleep (1st-level MU)                                                                      |
| 90     | Slow Poison (2nd-level druid)                                                             |
| 91     | Solid Fog (4th-level illusionist)                                                         |
| 92     | Spectral Force (3rd-level illusionist)                                                    |
| 93     | Spook (1st-level illusionist)                                                             |
| 94     | Stone to Flesh (6th-level MU)                                                             |
| 95     | Time Flow (5th-level illusionist)                                                         |


77-table-1.md

|   d100 | Result                                      |
|-------:|:--------------------------------------------|
|     96 | Triggered Illusion (6th-level illusionist)  |
|     97 | Veil of Abandonment (4th-level illusionist) |
|     98 | Wall of Fog (1st-level illusionist)         |
|     99 | Warp Wood (2nd-level druid)                 |
|    100 | Water Breathing (3rd-level MU)              |


77-table-2.md

| d100   | Result                                                                                  |
|:------ |:--------------------------------------------------------------------------------------- |
| 1-30   | Arcane                                                                                  |
| 31-60  | Divine                                                                                  |
| 61-70  | School (healing, divination, alteration, etc.)                                          |
| 71-80  | Specific spells (ESP does not work within the radius, etc.)                             |
| 81-90  | Spells with elemental affinity (fire, cold, etc.)                                       |
| 91-98  | Spells interacting  with  Alignment (detect evil/good, protection from evil/good, etc.) |
| 99-100 | All magic.                                                                              |


77-table-3.md

| d10   | Result   |
|:------|:---------|
| 1-2   | 25%      |
| 3-4   | 50%      |
| 5-6   | 75%      |
| 7-8   | 100%     |
| 9     | 125%     |
| 10    | 150%     |


77-table-4.md

| d100   | Result                                                       |
|:-------|:-------------------------------------------------------------|
| 1-13   | Have durations increased (1-3) or decreased (4-6).           |
| 14-26  | Have  ranges  increased  (1-3)  or  decreased (4-6).         |
| 27-39  | Have their area of effect increased (1-3) or decreased (4-6) |
| 40-53  | Have variables increased (1-3) or decreased (4-6).           |
| 54-67  | Have variables maximized (1-3) or minimized (4-6)            |
| 68-81  | Are more potent (1-3) or less potent (4-6).                  |
| 82-90  | Are easier to cast (1-3) or more difficult to cast (4-6).    |
| 91-93  | Are suppressed (1-3) or enhanced (4-6).                      |
| 94-95  | Null-magic.                                                  |
| 96-97  | Wild magic.                                                  |
| 98-99  | Roll twice, ignoring results of 98-100.                      |
| 100    | Roll three times, ignore results of 98-100.                  |


78-table-1.md

| d100   | Result      |
|:-------|:------------|
| 1-20   | 1d10 rounds |
| 21-40  | 1d6 turns   |
| 41-60  | 1d20 hours  |
| 61-80  | 1d8 days    |
| 81-90  | 1d4 weeks   |
| 91-100 | 1d12 months |


78-table-2.md

| d100                  | Result                                              |
|:----------------------|:----------------------------------------------------|
| 1-70                  | Two ley lines                                       |
| 71-95 Three ley lines |                                                     |
| 96-99                 | Four ley lines                                      |
| 100                   | Five  (1-3),  six  (4-5),  or  seven  (6) ley lines |


79-table-1.md

| d100   | Result                                                                                  |
|:------ |:--------------------------------------------------------------------------------------- |
| 1-25   | Increased (1-3)/decreased (4-6) vision                                                  |
| 26-50  | Increased (1-3)/decreased (4-6) sound                                                   |
| 51-75  | See around corners/obstacles                                                            |
| 76-95  | Distance between points is distorted, taking more (1-3)/less (4-6) time to move between |
| 96-100 | Gravity is non-standard                                                                 |