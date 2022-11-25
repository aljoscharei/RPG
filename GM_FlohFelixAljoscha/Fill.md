## Current position:
[[#Infrastructure]]
[[#Structures]]
[[#Resources]]


## Master Table
1.1 Feature Type `dice: [[Fill#^FeatureNoLairs]]`

| dice: 1d20 | Result                                                                    |
| ---------- | ------------------------------------------------------------------------- |
| 1-4        | Geologic Feature `dice: [[Fill#^GeologicFeature]]` |
| 5-8        | Structure `dice: [[Fill#^StructuresMaster]]`                                                                |
| 9-12       | Resource [[#Resources]]                                                                 |
| 13         | Hazard [[#Hazard]]                                                                   |
| 14         | Sign                                                                      |
| 15         | Dungeon                                                                   |
| 18         | Settlement                                                                |
| 20         | Magic                                                                     |
| 16-17      | Terrain `dice: [[Fill#^TerrainType]]`                                                                  |
| 19         | Water                                                                     |
^FeatureNoLairs

### Geologic

| dice: 1d6 | Result                                                                                                                                                                                                                                            |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1         | Change in Elevation. `dice: [[Fill#^hiLow]]` of `dice: [[Fill#^ElevationYards]]` `dice: [[Fill#^ElevationType]]`. The Area is `dice: [[Fill#^ElevationArea]]`. The Terrain is `dice: [[Fill#^elevationTerrain]]` comparing to surrounding Terrain |
| 2         | Soil `dice: [[Fill#^SoilApprearance]]` The soil is `dice: [[Fill#^SoilFecundity]]`, `dice: [[Fill#^SoilReasonFecundity]]`                                                                                                                                                                                                                                            |
| 3         | Terrain                                                                                                                                                                                                                                           |
| 4         | Caves. The cave has `dice: [[Fill#^CaveEntrances]]`.One Entrance is `dice: [[Fill#^TypeCaveEntrance]]`. There are `dice: [[Fill#^NumberChambers]]`. Is the water in the cave? `dice: [[Fill#^caveWater]]`                                         |
| 5         | Rock `dice: [[Fill#^typeRocks]]`                                                                                                                                                                                                                                              |
| 6         | Water                                                                                                                                                                                                                                             |
^GeologicFeature

#### Caves
Caves, obviously, are located below the ground and so are not always visible. Use the following rules to determine what the cave looks like. Note that any hex that has caves present gains the “Hazard (Sinkhole)” feature on a roll of 1 in 6 in the subhex containing the cave and the six subhexes around it. In addition, the vast majority of the time a cave system will be inhabited by a monster of some kind, even if it is not normally open to the surface world. There is a 1 in 20 chance per cave that it is totally uninhabited, with a further 1-3 in 6 chance that the cave is uninhabited for a specific reason (the air within is poisonous, the rock emits strong radiation, difficult to reach, etc.).

12-table-3.md

| d100  | Result                  |
|:----- |:----------------------- |
| 1-10  | no surface entrances    |
| 11-50 | 1 entrance              |
| 51-75 | 2 entrances             |
| 76-90 | 3 entrances             |
| 91-99 | `dice: 1d4+2` entrances |
| 100   | `dice: 2d4+2` entrances |
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
| 1-35   | A  number  of  smaller  rocks  (roll  `dice: 1d6`-1  to indicate the average diameter, in feet), with a  density  of  `dice: 3d10`  per  `dice: 1d20`×100  sq.  ft.  A result of 0 indicates the rocks are, on average, smaller than a foot in diameter.`dice: [[Fill#^AreaRocks]]` `dice: [[Fill#^rocksUnusual]]`                                                                                                                                                                                                  |
| 36-70  | a  smaller  number  of  larger  rocks,  with  an average diameter of 3d6 feet and a density of 1d4 per 1d20×100 feet. `dice: [[Fill#^AreaRocks]]` `dice: [[Fill#^OriginRocks]]` `dice: [[Fill#^rocksUnusual]]`                                                                                                                                                                                                                                                                                                            |
| 71-100 | an  outcropping  of  rock.  If  the  outcropping occupies  a  single  subhex  there  is  only  one; if  multiple  subhexes  there  is  a  chance  each subhex will have (1-3) a single outcropping, (4-5) 1d4 outcroppings (depending on overall  size),  or  (6)  the  outcroppings  join together  to  form  one  massive  outcropping that covers the entire area.  To determine the size of the outcropping roll below: `dice: [[Fill#^OutcroppingSize]]`, `dice: [[Fill#^OutcroppingArea]]` |
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

| d100  | Result                 |
|:----- |:---------------------- |
| 1-60  | 1 subhex               |
| 61-89 | `dice: 1d4+1` subhexes |
| 90-96 | `dice: 3d8` subhexes   |
| 97-99 | 1 hex                  |
| 100   | `dice: 1d4+1` hexes    |
^OutcroppingArea

If the rocks are not an outcropping they will cover an area of . . .
14-table-1.md



| d100  | Result                          |
|:----- |:------------------------------- |
| 1-30  | `dice: 1d4`x100 square feet     |
| 31-50 | `dice: 2d6`x500 square feet     |
| 51-65 | `dice: 3d8`x1,000 square feet   |
| 66-80 | `dice: 4d10`x10,000 square feet |
| 81-90 | `dice: 1d4` subhexes            |
| 91-95 | `dice: 3d6` subhexes            |
| 96-99 | `dice: 4d8` subhexes            |
| 100   | `dice: 1d4` hexes               |
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

| dice: 1d36 | result                                                                                                                                                                                |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-3        | The rocks have been written on. The writing is `dice: [[Fill#^writingRockHow]]`, Further, the writing will be on `dice: [[Fill#^WritingRockAmount]]`,`dice: [[Fill#^writingContent]]` |
| 4-5        | The rocks are arranged in a specific pattern. The pattern can `dice: [[Fill#^patternPerspective]]` , `dice: [[Fill#^patternFunction]]`                                                |
| 6          | The Rocks are Magical. Refer to the section on Magical Features.                                                                                                                      |
| 7-36       | There is nothing unusual about the rocks                                                                                                                                              |
^rocksUnusual



| dice: 1d6 | result                                                 |
| --------- | ------------------------------------------------------ |
| 1-2       | carved into the stone,                                 |
| 3-4       | written on the surface with some substance,            |
| 5         | patterned in lichen or moss, or                        |
| 6         | appears organically in the surface of the rock itself. |
^writingRockHow



| dice: 1d6 | result            |
| --------- | ----------------- |
| 1-3       | one single stone  |
| 4-5       | 1d20+1 stones     |
| 6         | all of the stones |
^WritingRockAmount

The writing 
| dice: 1d6 | result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1         | Is meaningless, obscene or pornographic graffiti.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| 2         | Contains the formula to a spell (1-4) or magical item (5-6). It takes 1d8 weeks plus one day per additional stone containing the writing to decipher and understand what is scribed upon it.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 3         | A prophecy, concerning events that are yet to come (1-4) or have already passed (5-6). There’s a 1-2 in 6 chance the prophecy is wrong.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 4         | A map. On a 1-2 it’s a treasure map (roll on the Scrolls treasure table, treating all non treasure map results as a reroll), 3-4 it’s a map of the surrounding area, 5 it’s a map to an undiscovered/unknown area (1-2 in 6 chance of being in another plane or dimension), or 6 a map of a random location.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 5         | There’s a small crevice in the rock, and if the adventurers write a question on a slip of paper (1-2 in 6 chance that the question must be asked in a specific language, (3-4) written in the asker’s blood, or (5-6) accompanied by a gift), slip it into the crevice, and return the next day the writing will reform itself as an answer to the question posed (treat as 1-3 augury, 4-5 divination, or 6 commune, all as if cast by a cleric of level 6+1d8).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| 6         | The writing is 1 a record of historical events (see Monuments, p. 17), 2 a warning about dangers (1-4 current, 5-6 past and no longer relevant) in the area, 3 a personal missive directed to one of the adventurers (1-3 chance of being accurate, from a dead relative or friend. There’s a 1-2 chance it will contain advice about upcoming events, otherwise it will just be the friend or relative saying hello), 4 a single letter per stone (see above to determine the number of stones with writing on them), arranged in a random fashion (the letters, when sorted, spell out 1-2 a dirty word, 3-4 the name of an ancient king or magician, 5 the name of an ally of the party who means to betray them, or 6 the true name of a demon or fairy that can be used to bind said creature), 5 assembly directions (if the stones are arranged according to the directions written upon them they will create 1-2 a sculpture, 3-4 a crude dwelling, 5 a portal that functions as a gate to another world, or 6 a circle 1d20+10 feet in diameter, inside which the adventurers may camp without fear of wandering monsters. In the last two instances the effects last for 1 1d4 uses (camping 8 hours counts as a “use”), 2 1d4 hours, 3 3d4 hours, 4 1d4 days, 5 1d4 weeks, 6 permanently) or 6 something else of the Referee’s choosing. |
^writingContent

4-5) The rocks are arranged in a specific pattern. The pattern can


| dice: 1d6 | result                        | 
| --------- | ----------------------------- |
| 1-4       | only be discerned from above  |
| 5-6       | is obvious from ground level. |
^patternPerspective

The pattern will be one of the following 


| dice: 1d108 | result                                                                                                                                                                                                                           |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-6         | There is power within the pattern, but it is not clear what it is. It takes 1d8 days of study to determine what the pattern does. It is a ward against something (roll on the Scrolls table to determine what it wards against), |
| 7-9         | There is power within the pattern, but it is not clear what it is. It takes 1d8 days of study to determine what the pattern does. functions as a gate to another place in this world,                                                                                                                                                                              |
| 10-11       | There is power within the pattern, but it is not clear what it is. It takes 1d8 days of study to determine what the pattern does. functions as a gate to a place in another world or dimension, or                                                                                                                                                                 |
| 12          | functions as a gate to another time                                                                                                                                                                                              |
| 13-14       | functions to alter the surrounding weather by moderating,                                                                                                                                                                        |
| 15-16       | functions to alter the surrounding weather by intensifying, or                                                                                                                                                                   |
| 17-18       | functions to alter the surrounding weatherby attracting a certain phenomenon)                                                                                                                                                    |
| 19-24       | it acts as a prison, containing a powerful creature or creatures (with a combined HD total of 10d10)                                                                                                                             |
| 25-30       | acts as a focus for ley line energy (see the section on Magic, p. 66, as well as Hex 13.22 for more information on ley lines. There’s a 1-3 in 6 chance the ley line it once focused has since shifted position)                 |
| 31-36       | is an artifact designed to cast a permanent spell over a larger area.                                                                                                                                                            |
| 37-72       | The pattern is mundane in nature, forming a shape or image with little to no significance except to its executor.                                                                                                                |
| 73-108      | The pattern is of a random shape or arrangement, determined by the whim of of a mad artist, whimsical deity or capricious spirit.                                                                                                |
^patternFunction

#### Soil
The soil here differs from the surrounding soil. Roll below to determine the exact nature of the change.

Appearance (1d6) . . .

On a roll of

| dice: 1d36 | Result                                                                                                                           |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 1-12       | the soil superficially resembles the surrounding soil,                                                                           |
| 13-30      | it has a different appearance (color, texture, etc.).                                                                            |
| 31-36      | There’s a further 1 in 6 chance that if the soil has a different appearance it will be unusual or unnatural in color or texture. |
^SoilApprearance


Fecundity (1d6) . . .

The soil is 

| dice: 1d6 | result                                                                                                                                                                                                               |
| --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-2       | as productive as the surrounding soil,                                                                                                                                                                               |
| 3-4       | more productive, More productive soil is characterized by riotous plant life; the grass is greener and more lush, the trees quiver with energy and fruits and vegetables grown here will produce their maximum yield |
| 5-6       | less productive. .  Less productive soil is barren or almost bare, with whatever plants do survive being unusually hardy, stunted and sick-looking. Seeds do not take, regardless of how much the farmer tends       |
^SoilFecundity

If a third or more of the subhexes in this hex are more productive, increase the land value of the overall hex by 1 (refer to p. 23 of Domain Building for a discussion of land value).

15-table-1.md

| d6   | Result                                                                                                                                                                                                                                                        |
|:-----|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-3  | The soil has the special quality due to a mineral, nutrient or other naturally occurring feature.                                                                                                                                                             |
| 4-5  | The soil is different because of artificial means (perhaps it is terraced or fertilized or has been poisoned  by  an  enemy).  If  this  is  the  case, further  labor  can  altered  it  from  its  current state at a cost of 1,000 gp per subhex affected. |
| 6    | The soil is as it is as the result of a curse or beneficial  spell.  It  is  possible  to  remove  the curse or spell.                                                                                                                                        |
^SoilReasonFecundity



### Structures
This section covers all sorts of structures that can be found in the wilderness, from simple lean-to shelters to elaborate mansions and free-holds, from abandoned shepherd huts to ruined castles and keeps.

Unless otherwise stated,
structures in Civilized areas have a 1-5 in 6 chance of being used for their intended purposes, 
those in Borderlands have a 1-3 in 6 chance, and t
hose in Wilderness areas have a 1-2 in 6 chance. F
or a discussion of the differences between Civilized, Borderlands, and Wilderness hexes refer to p. 15 of the supplement Domain Building.

Structures used for their intended purpose will not be abandoned, or lairs for monsters, or otherwise unusable.

If structures are abandoned or no longer in use they can potentially be used either to house lairs of monsters that have already been rolled for (see Lairs, above) *or* they can be used to introduce a new lair. It is up to the Referee to decide how they want to populate structures within a hex.

17-table-2.md

| d10 | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|:--- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | Burial Grounds. Its Size is `dice: [[Fill#^BurialGroundSize]]`. Each dead occupies `dice: 1d20+15` sq. ft. The dead are buried.. `dice: [[Fill#^HowBuried]]`. How long  have they been dead: `dice: [[Fill#^howlongDead]]`. The dead are: `dice: [[Fill#^deadAncestry]]`, `dice: [[Fill#^buriedceremony]]`  `dice: [[Fill#^buriedTemple]]`.                                                                                                                                                                                                                                                                                                                                                   |
| 2   | Monuments to `dice: [[Fill#^MonumenttoWhom]]` `dice: [[Fill#^monumentShape]]`, `dice: [[Fill#^MonumentSize]]`, `dice: [[Fill#^monumentHollow]]`, `dice: [[Fill#^monumentAge]]`, `dice: [[Fill#^monumentMaterial]]` , `dice: [[Fill#^isSpecialQuality]]`                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 3-5 | Dwellings `dice: [[Fill#^dwellingInhabitants]]`, age `dice: [[Fill#^monumentAge]]`, condition `dice: [[Fill#^dwellingCondition]]`, The dwelling is made of . . . `dice: [[Fill#^dwellingMaterials]]` , its size is:  `dice: [[Fill#^dwellingSize]]`                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| 6   | Fortificaton. A `dice: [[Fill#^fortificationType]]` made of `dice: [[Fill#^fortificationMaterial]]`. It is `dice: [[Fill#^dwellingCondition]]` its age is `dice: [[Fill#^monumentAge]]`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 7-8 | Infrastructure `dice: [[Fill#^InfrastructureType]]`,                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 9   | Barriers `dice: [[Fill#^barriertype]]`, Barriers, if the adventurers insist on continuing on their path, will slow progress by `dice: [[Fill#^BarrierIntensity]]`, Each barrier affects a “zone”, or a certain area. The smallest area a zone can affect is a single subhex. Roll below to determine the size of the zone `dice: [[Fill#^BarrierZone]]`. Barriers can be overcome or avoided through spells, clever thinking, or simple brute force or ignorance. Labor can be used to clear a forest of hampering underbrush or to build a bridge across a ravine, as a permanent solution. Powerful magics may be needed to permanently eliminate other barriers, both magical and mundane. |
| 10  | Dungeons                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
^StructuresMaster

---


#### Burial Ground
Structures in this category range from simple wooden or stone grave markers to large mausoleums and sprawling necropolises. Roll below to determine what is found.


There’s a 1-3 in 6 chance the dead have been buried as part of a religious ceremony (see Unhallowed Ground, below). This chance is increased by 1 in Civilized hexes, and again by 1 if the grave is marked or they were ritually exposed. The chance is decreased by 1 in Wilderness hexes, and again if the dead weren’t buried, were buried in unmarked graves, or were killed as a punishment.

In Civilized hexes there’s a 1-3 in 6 chance the burial ground is part of a temple or sacred ground, and a further 1-3 in 6 chance that one or more priests or guardians stand vigil over the dead. In Borderlands these chances are reduced to 1-2 in 6 and 1-2 in 8, respectively, and in Wilderness hexes they are reduced further to 1 in 8 and 1 in 12, respectively.

As a general rule of thumb each body occupies between 1d20+15 sq. ft. for purposes of determining the size of the burial grounds. Add modifiers as needed, and only roll once to determine the average size, then apply that to all the bodies within. For instance, bodies interred in a mausoleum take up less space than, say, bodies left to rot after a battle.

In Civilized hexes there’s a1-3 in 6 chance the burial ground is part of a temple or sacred ground, and a further 1-3 in 6 chance that one or more priests or guardians stand vigil over the dead. In Borderlands these chances are reduced to 1-2 in 6 and 1-2 in 8, respectively, and in Wilderness hexes they are reduced further to 1 in 8 and 1 in 12, respectively.


As a general rule of thumb each body occupies between 1d20+15 sq. ft. for purposes of determining the size of the burial grounds. Add modifiers as needed, and only roll once to determine the average size, then apply that to all the bodies within. For instance, bodies interred in a mausoleum take up less space than, say, bodies left to rot after a battle.




17-table-1.md

| dice: d100 | Result               |
|:---------- |:-------------------- |
| 1-30       | Single Grave         |
| 31-60      | `dice: 1d4+1` dead   |
| 61-75      | `dice: 3d4` dead     |
| 76-85      | `dice: 4d6` dead     |
| 86-96      | `dice: 5d10` dead    |
| 96-97      | `dice: 6d20` dead    |
| 98         | `dice: 7d100` dead   |
| 99         | `dice: 10d100`       |
| 100        | `dice: 100d100` dead |
^BurialGroundSize

How are the dead buried?

18-table-2.md

| d100  | Result                                                                                                        |
|:----- |:------------------------------------------------------------------------------------------------------------- |
| 1-25  | They’re not Buried.  The dead are left exposed to the elements as they fell. `dice: [[Fill#^diedofviolence]]` |
| 36-30 | Buried in a mass grave                                                                                        |
| 31-60 | Wooden markers The markers `dice: [[Fill#^graveWriting]]`                                                     |
| 61-75 | Stone tombstones. The stones `dice: [[Fill#^graveWriting]]`                                                   |
| 76-80 | Mausoleums or crypts. Is there writing?  `dice: [[Fill#^graveWriting]]`                                       |
| 81-86 | Barrows or burial mounds                                                                                      |
| 87-90 | Ritually exposed to the elements                                                                              |
| 91-95 | As punishment (gibbets, crucifixion, gallows, etc.)                                                           |
| 96-99 | In unmarked graves.                                                                                           |
| 100   | Unique or magically (turned to stone or trees, frozen in blocks of ice, embedded in amber, etc.)              |
^HowBuried

`dice: [[Fill#^buriedceremony]]`

Have the dead been buried with a ceremony?

| result |                                                               |
| ------ | ------------------------------------------------------------- |
| 1-3    | the dead have been buried as part of a religious ceremony     |
| 4-6    | the dead have not been buried as part of a religious ceremony |

^buriedceremony


This chance is increased by 1 in Civilized hexes, and again by 1 if the grave is marked or they were ritually exposed. The chance is decreased by 1 in Wilderness hexes, and again if the dead weren’t buried, were buried in unmarked graves, or were killed as a punishment.

| dice: 1d4 | result                                                                                                                                                                                                           |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-2       | the burial ground is not part of a temple or sacred ground. The ground is `dice: [[Fill#^unhallowedNoTemple]]` This chance increases by 1 for every 50 bodies interred in the area, up to a maximum of 1-5 in 6. |
| 3         | the burial ground is part of a temple or sacred ground `dice: [[Fill#^unhallowedTemple]]`                                                                                                                        |
| 4         | the burial ground is part of a temple or sacred ground and one or more priests or guardians stand vigil over the dead. `dice: [[Fill#^unhallowedTemple]]`                                                        |
^buriedTemple

| dice: 1d6 | result                                                                                                                                                                            |
| --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-5       | hallowed                                                                                                                                                                          |
| 6         | unhallowed. The forces of Chaos and undeath rule supreme in unhallowed ground. An unhallowed burial site will have qualities from the below table. `dice: [[Fill#^1-3qualities]]` |

^unhallowedTemple

| dice: 1d6 | result                                                                                                                                                                           |
| --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-4       | hallowed                                                                                                                                                                         |
| 5-6       | unhallowed The forces of Chaos and undeath rule supreme in unhallowed ground. An unhallowed burial site will have qualities from the below table. `dice: [[Fill#^1-3qualities]]` |

^unhallowedNoTemple


| dice: 1d6 | result                                                                                                            |
| --------- | ----------------------------------------------------------------------------------------------------------------- |
| 1-3       | `dice: [[Fill#^unhallowedQualities]]`                                                                             |
| 4-5       | 1:`dice: [[Fill#^unhallowedQualities]]` 2: `dice: [[Fill#^unhallowedQualities]]`  If duplicates are rolled the effects stack unless otherwise noted.                                      |
| 6         | 1: `dice: [[Fill#^unhallowedQualities]]` 2: `dice: [[Fill#^unhallowedQualities]]` 3: `dice: [[Fill#^unhallowedQualities]]`  If duplicates are rolled the effects stack unless otherwise noted. |
^1-3qualities

| unhallowed qualities                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| The dead walk. Those that die within unhallowed ground for every night their body remains within the borders.  `dice: [[Fill#^deadRise]]`                                                                                                                                                                                                                                                                                                                                                                                                     |
| The dead resist. `dice: [[Fill#^deadresist]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| The dead persist. Undead that are created within the unhallowed ground (whether “naturally” or due to spells such as animate dead) do so with 1d10 hit points per HD rather than 1d8. There’s a further 1-2 in 6 chance that one of the following occurs `dice: [[Fill#^deadPersistTable]]`                                                                                                                                                                                                                                                   |
| The dead protest. Both clerical and natural healing is stifled within the unhallowed ground. Natural healing does not occur, and magical healing is minimized (roll twice, taking the lower result).                                                                                                                                                                                                                                                                                                                                          |
| The evil permeates. The entire unhallowed area radiates evil. Spells that detect evil or alignment do not function due to the aura of Chaos that suffuses the space, and spells or items that ward or rely on the identification of alignment also do not function. Lawful-aligned creatures are uneasy in this place, taking a –1 penalty to surprise rolls, and having difficulty sleeping. Each night they try to sleep in the area they make a Save v. Spells; failure indicates they do not sleep soundly enough to regain hp or spells. |
| The dead hunger. If an undead creature rolls a 19 or 20, their blows automatically inflict maximum damage. There’s an additional 1-2 in 6 chance that saving throws made by non-Chaotic creatures within the unhallowed ground are done with disadvantage (rolling twice and taking the worse result).                                                                                                                                                                                                                                        |
| The dead corrupt. Magical items that remain within the unhallowed ground for more than 1 week have a 1-2 in 6 chance of being corrupted by the Chaotic energies. Corrupted items will be cursed in a manner left up to the Referee.                                                                                                                                                                                                                                                                                                           |
| The dead speak. A soft susurrus of damned voices fills the unhallowed ground. Non-Chaotic creatures suffer a –1 penalty to initiative and surprise and must Save v. Spells each time they enter the ground or be affected as per `dice: [[Fill#^blightConfusea]]`                                                                                                                                                                                                                                                                             |

^unhallowedQualities



| dice: 1d6 | result                              |
| --------- | ----------------------------------- |
| 1-4       | the blight spell (reverse of bless) |
| 5-6       | confusion spell                         |

^blightConfusea


| dice: 1d36 | result                 |
| ---------- | ---------------------- |
| 1-30       | dead don't rise        |
| 31-33      | dead rise as skeletons |
| 34-35      | dead rise as zombies   |
| 36         | dead rise as ghouls    |
^deadRise


| dice: 1d4 | result                                                                                                                                                                                            |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1         | Undead regenerate 1 hp per round while within the unhallowed area.                                                                                                                                |
| 2         | The first time an undead creature is reduced to 0 hp they instead remain at 1 hp.                                                                                                                 |
| 3         | An undead creature destroyed within an unhallowed area will reform over a period of  `dice: [[Fill#^deadReform]]` unless their remains are burned, blessed by a cleric, or removed from the area. |
| 4         | Undead created within the area have an AC that is `dice: [[Fill#^deadAC]]` better than normal.                                                                                                    |

^deadPersistTable


| dice: 1d6 | result |
| --------- | ------ |
| 1-3       | 1      |
| 4-5       | 2      |
| 6         | 3      |
^deadAC

| dice: 1d6 |                                                             |
| --------- | ----------------------------------------------------------- |
| 1-3       | Undead within unhallowed ground are treated as having +1 HD |
| 4-5       | Undead within unhallowed ground are treated as having +2 HD |
| 6         | Undead within unhallowed ground are treated as having +3 HD |
^deadresist

| dice: 1d6 | result              |
| --------- | ------------------- |
| 1         | `dice: 1d6` rounds  |
| 2-3       | `dice: 1d6` minutes |
| 4-5       | `dice: 1d6` hours   |
| 6         | `dice: 1d6` days    |
^deadReform






| dice: 1d2 | Died of violence                                                                                                                                                                             |
| --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1         | they died of violence from a creature that appears on the wandering monster table for the hex. A careful examination of the bodies may give a clue as to what threat waits to be discovered. |
| 2         | they died without violence                                                                                                                                                                                             |
^diedofviolence

 Graves with permanent markers
| dice: 1d20 | result                                                            |
| ---------- | ----------------------------------------------------------------- |
| 1-10       | have no writing                                                        |
| 11-12      | have some sort of writing describing  who is buried,              |
| 13-14      | have some sort of writing describing when they were born and died |
| 15         | have some sort of writing describing how they died,               |
| 16         | some other fact about them,                                       |
| 17         | two of the previous                                               | 
| 18         | three of the previous, or                                         |
| 19-20      | the writing is illegible.                                         |
^graveWriting




How long  have they been dead.?

18-table-3.md

| dice: d200 | Result                                                                                                                          |
|:---------- |:------------------------------------------------------------------------------------------------------------------------------- |
| 1-5        | `dice: 1d4` days                                                                                                                |
| 6-10       | `dice: 1d4` weeks                                                                                                               |
| 11-20      | `dice: 1d12` months                                                                                                             |
| 21-30      | `dice: 1d10` years                                                                                                              |
| 31-40      | `dice: 2d20` years                                                                                                              |
| 41-50      | `dice: 5d20` years                                                                                                              |
| 51-75      | `dice: 10d20` years                                                                                                             |
| 76-99      | `dice: 10d100` years                                                                                                            |
| 100        | `dice: 1d4` millennia                                                                                                           |
| 101-200    | the dead in the graveyard span a considerable length of time. If this is the case roll twice, above, to determine the time span |
^howlongDead


The dead will be . . .

| d100   | Result                                    |
|:------ |:----------------------------------------- |
| 1-50   | Human (or whatever the dominant race is.) |
| 51-75  | Demi-human (elf, dwarf, gnome, etc.)      |
| 76-90  | Humanoid                                  |
| 91-95  | Monster                                   |
| 96-100 | Mix of races                              |
^deadAncestry


#### Monuments:
The civilizations of the past leave behind great works whose function is to memorialize great heroes and rulers, portentous events and defining battles, while current rulers do the same to make their glory known to their subjects. Monuments can also be alien or inscrutable in nature, of uncertain purpose or provenance, or even simple structures erected by the common folk to commemorate certain events.

Monuments fall into several different categories. . .

20-table-2.md

| d100   | Result                                                                                                           |
|:-------|:-----------------------------------------------------------------------------------------------------------------|
| 1-25   | Built  to  honor  the  dead  (usually  fallen  in battle or disaster)                                            |
| 26-50  | Built to honor an event (such as a battle, the signing of a treaty, the birth of a ruler, etc.).                 |
| 51-75  | Built to honor an individual (such as a ruler, powerful mage, etc.)                                              |
| 76-85  | Built to honor a concept (such as Law or Chaos)                                                                  |
| 86-95  | Built to honor a religion or deity. Refer to the section on shrines on p. 34                                     |
| 96-100 | Built  to  house  an  object  or  person  (such as  an  artifact  or  relic,  or  an  emperor’s burial chambers) |
^MonumenttoWhom

Monuments built to honor the dead typically do not have any dead interred within them, but occasionally will contain relics or memento mori in some capacity.

The monument will take the shape of . . .

20-table-3.md

| d600    | Result                                                                                                                              |
|:------- |:----------------------------------------------------------------------------------------------------------------------------------- |
| 1-100   | A statue (1-4). It is a `dice: [[Fill#^petrified]]`, `dice: [[Fill#^defaced]]` `dice: [[Fill#^StatuesDepict]]`,                                                       |
| 101-150 | multiple statues (5-6). It is a `dice: [[Fill#^petrified]]`, `dice: [[Fill#^defaced]]`                                              |
| 151-225 | An obelisk (1-3) Obelisks are rectangular columns with a pyramidal cap                                                              |
| 226-275 | column singular columns are typically round                                                                                         |
| 276-300 | regular columns found in clusters of `dice: 1d8+1`.                                                                                 |
| 301-450 | Megalith                                                                                                                            |
| 451-480 | Arch (1-3),                                                                                                                         |
| 481-500 | building (4-5) or                                                                                                                   |
| 501-510 | freeform structure (6)                                                                                                              |
| 511-520 | Pyramid  (1-2),                                                                                                                     |
| 521-530 | terraced  pyramid  (3-4)  or                                                                                                        |
| 531-540 | earthen mounds `dice: [[Fill#^earthenMound]]`                                                                                       |
| 541-570 | Fountain or Water feature Fountains or similar water features are occasionally built as memorials, especially by cultures for which |
| 571-600 | Magical or Unique material/form. Size: ``                                                                                                     |
^monumentShape

Obelisks are rectangular columns with a pyramidal cap, while columns are typically round. There’s a 1-2 in 6 chance that regular columns are found in clusters of 1d8+1.

Megaliths are large stones erected as monuments or ritual foci. They are either single stones, called menhirs, potentially arranged in a pattern with other menhirs, or arranged to form a structure (such as Stonehenge) or even rudimentary shelter.

Arches, buildings, and other abstract structures are designed as larger memorial complexes. Think of l’Arc de Triomph in Paris, or the Vietnam Memorial Wall in Washington DC.

Pyramids, stepped pyramids, and earthen mounds are all similar in appearance but built using different techniques and levels of technology. Earthen mounds will be 



| dice: 1d6 | result                        |
| --------- | ----------------------------- |
| 1-2       | roughly pyramidal in shape,   |
| 3-4       | another geometric shape       |
| 5-6       | an abstract or symbolic form. |
^earthenMound


| dice: d300 | result                            |
| ---------- | --------------------------------- |
| 1          | Petrified person with petrified Treasure |
| 2-3        | Petrified person without Treasure        |
| 4-300      | normal statue                     |
^petrified

| dice: 1d12 | result                                               |
| ---------- | ---------------------------------------------------- |
| 1          | statue’s features will have been erased by time      |
| 2          | statue’s features will have been erased by vandalism |
| 3-12       | features intact                                                     |
^defaced

This chance increases by 1 in Borderlands hexes or 2 in Wilderness hexes.

There’s a 1 in 100 chance that statues discovered in an area are in fact the petrified remains of once-living beings, turned to stone either by monsters such as basilisks, curses, or stray magical effects. If this is the case there’s a 1-2 in 6 chance that level appropriate treasure can be found on the statue if it were un-petrified.


20-table-1.md
Statues will depict: 

| d100   | Result                            |
|:-------|:----------------------------------|
| 1-40   | Humans                            |
| 41-75  | Demi-humans                       |
| 76-90  | Humanoids                         |
| 91-98  | Other Races (dragon, giant, etc.) |
| 99-100 | Abstract concepts                 |
^StatuesDepict


The last category is all-encompassing. Perhaps the memorial is a permanent illusion that constantly replays the final moments of a decisive battle, or a field of magical energy that causes those within it to experience a specific emotion. Memorials could also be abstract works of art like the chalk figures of England, or the Nazca lines of Peru.

21-table-3.md

| d100   | Result                                                                                                                                                                                                                                                                       |
|:-------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1      | Small. probably erected by a race of Micronians or perhaps awakened animals.                                                                                                                                                                                                 |
| 2-60   | Medium. sized or scaled for Men (statues will be approximately human height, buildings and other structures scaled for human habitation).                                                                                                                                    |
| 61-90  | Large. sized for ogres and such. Statues will be approximately 8-10’ tall, obelisks around 20-35 feet. There is a 1-2 in 6 chance that the monuments are actually designed by a large race; the other 66% of the time they’re built by human-sized creatures with big ideas. |
| 91-99  | Giant-sized.  Statues  will  be  approximately 11-20’ tall,  obelisks  and  columns  around 36-50 feet. There is a 1 in 6 chance that the monuments are actually designed by a large race;  the  rest  of  the  time  they’re  built  by human-sized folks with big ideas.   |
| 100    | Enormous.  These  monuments  are  so  large they boggle the mind and are either built by creatures larger than the largest giants (1 in 6 chance) or by large kingdoms and empires (such as the Pyramids at Giza).                                                           |
^MonumentSize

There’s a 1 in 6 chance 

| dice: 1d6 |                                                                                                                                                                                                        |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1         | the monuments have internal space (if appropriate). Monuments with internal spaces will contain `dice: 1d4` chambers, with size obviously being a limiting factor.  `dice: [[Fill#^MonumentEntrance]]` |
| 2-6       | monument is solid                                                                                                                                                                                      |
^monumentHollow


| dice: 1d4 |                                             |
| --------- | ------------------------------------------- |
| 1         | the entrance is visible on a roll of 1-2,   |
| 2         | visible but locked on a roll of 3-4,        |
| 3         | concealed but unlocked on a roll of 5-6, or |
| 4         | concealed and locked on a roll of 7-8.      |
^MonumentEntrance




If a monument contains internal space use the Dungeon Stocking Table on p. 225 of OSE core to determine what can be found within. Roll 1d12 to determine the “level” of the dungeon for purposes of stocking with monsters and treasure (p. 225 of OSE core gives the amount of treasure to be found):


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

* Roll for each treasure category twice, taking the lower of the two results. Ex. A treasure is to be found within, equivalent to that found on a level three dungeon. The Referee rolls 1d100 twice for each category listed (sp, gp, gems, jewelry, magic item), taking the lower result of each pair.

Monuments will be of the following age . . .

21-table-2.md

| d100   | Result                |
|:------ |:--------------------- |
| 1-10   | `dice: 1d10` years    |
| 11-50  | `dice: 10d10` years   |
| 51-95  | `dice: 10d100` years  |
| 96-100 | `dice: 10d1000` years |
^monumentAge

They will be constructed of . . .

21-table-4.md

| d100   | Result           |
|:-------|:-----------------|
| 1-20   | Wood/Bone/Brick  |
| 21-45  | Metal            |
| 46-95  | Stone            |
| 96-100 | Exotic Materials |
^monumentMaterial

There is a 1-3 in 6 chance that the monument is engraved with writing. If so, there’s a 1-2 in 6 chance that time and the elements have obscured most, if not all, of the writing, and a further 1-2 in 6 chance the language is dead and no longer known to Man.



There’s a further 1 in 20 chance that the monument possesses a special quality:

| dice: 1d20 | result                                   | 
| ---------- | ---------------------------------------- |
| 1          | `dice: [[Fill#^monumentSpecialQuality]]` |
| 2-20       | no special quality                       |
^isSpecialQuality

| dice: 1d6 |                                                                                                                                                                                                                                   |
| --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1         | The monument provides a clue to a mystery or points the way to something relevant: a buried treasure, a dungeon, an imprisoned efreet, etc.                                                                                       |
| 2         | The monument radiates magical energy and is the focal point of a randomly determined spell. The only way to end the spell’s effect is to destroy the monument.                                                                    |
| 3         | The monument is actually a device designed to capture ley line energy. There’s a 1-2 in 6 chance that the ley line has since shifted and energy is no longer being stored.                                                        |
| 4         | The monument serves as a prison for some powerful being.                                                                                                                                                                          |
| 5         | f touched or manipulated in a specific way the monument will provide a boon (1-3) or a bane (4-6). In the case of a boon there’s a 1-2 in 6 chance that a sacrifice (of blood, coin, magic, etc.) is required for it to function. |
| 6         | The monument is a portal to another plane. There’s a 1-2 in 6 chance it functions without effort, otherwise some ritual or spell is required for it to function.                                                                  |
^monumentSpecialQuality


---

#### Dwellings

The wilderness is filled with hovels, huts and houses erected by various peoples, either inhabited by the original builder, a recent arrival or completely abandoned.

The dwellings are . . .

22-table-1.md

| d100   | Result                                                                                                                                                                                                                                   |
|:-------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-25   | Inhabited by monsters. Roll on the wandering encounter  table  appropriate  for  the  area  to determine exactly what lives within.                                                                                                      |
| 26-60  | Uninhabited. If it is uninhabited there is a 1-2 in 6 chance of there being valuables within the house, with the following treasure type (1-A, 2-B, 3-C, 4-D, 5-E, 6-F). There is an additional 1-3 in 6 chance the treasure is trapped. |
| 61-100 | Inhabited  by the  original  builders (or the descendants/same race as the original builders).                                                                                                                                           |
^dwellingInhabitants


22-table-2.md

[[Fill#^monumentAge]]

The dwelling is in what condition? Subtract 1 from the roll for every 100 years of age, with a maximum modifier of –15:

22-table-3.md

| d100   | Result                       |
|:-------|:-----------------------------|
| 1-15   | Crumbling and falling apart. |
| 16-50  | In need of some repair.      |
| 51-85  | In relatively decent shape.  |
| 86-100 | Immaculately maintained.     |
^dwellingCondition


The dwelling is made of . . .

22-table-4.md

| d100   | Result                                                                                 |
|:-------|:---------------------------------------------------------------------------------------|
| 1-25   | Materials  found  locally  and  appropriate  for the surroundings.                     |
| 26-60  | Materials imported from afar.                                                          |
| 61-100 | Unique materials or those created by magic: a palace of glass, or amber, for instance. |
^dwellingMaterials

The materials used in the construction of a dwelling will be largely dependent upon the size and resident. For instance, most buildings in a forested hex might be log cabins with thatched roofs, inhabited by independent freeholders, while a retired adventurer might live in a wood-framed house with a cedar shake roof, and a noble’s manor may be stone with a slate roof. Most dwellings on a prairie may be sod, with larger/wealthier houses being wood, or perhaps brick or adobe.


23-table-4.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-10   | Tiny.  A  single-room  hut,  hovel  or  house. There’s  `dice: 1d6<3`  chance  the  dwelling  was designed to be temporary (such as a lean-to, hide tent, yurt, etc.). It’s been built to provide shelter, with no extraneous rooms.                                                                                                                                                                                                                                                                                                            |
| 11-30  | Small.  The dwelling has `dice: 1d3` rooms, potentially  with  a  sleeping  space  separate from the living space. There’s `dice: 1d6<2` chance the  dwelling is  surrounded  by  a  wall  or similar fortification.                                                                                                                                                                                                                                                                                                                                         |
| 31-75  | Medium.  The  dwelling  has  `dice: 1d4+1`  rooms and  is  generally  what  we  would  consider to  be  a  “house”  with  dedicated  rooms  for different purposes. There’s `dice: 1d6<3` chance the  dwelling is  surrounded  by  a  wall  or similar fortification. There’s `dice: 1d8<2` chance the dwelling is actually a fortified keep.                                                                                                                                                                                                                   |
| 76-95  | Large.  The  dwelling  has  `dice: 1d6+4`  rooms  and would  be  consistent  with  a large freehold supporting  several  families.  If  there  are  more than 6 rooms there’s `dice: 1d6<3` chance the rooms are  actually  divided  between  `dice: 1d2+1`  buildings, forming a compound. If all the rooms are in one building, there’s `dice: 1d6<3` chance the dwelling is surrounded by a wall, or if in multiple buildings there’s `dice: 1d6<4` chance of the same. There’s `dice: 1d8<2` chance the building is actually a keep, with a primarily defensive function. |
| 96-98  | Very Large. The dwelling has `dice: 1d12+5` rooms and  is  roughly  the  size  of  a  manor  house. There’s  a  `dice: 1d6<4`  chance that there  are `dice: 1d2+1`  outbuildings  surrounding  the  main house,  with  2d4  rooms  divided  amongst them. There’s a `dice: 1d8<4`chance the buildings are  surrounded  by  walls  or  other  defensive fortifications,  and  an  additional  `dice: 1d8<3` chance the building is actually a keep, with a primarily defensive function. |
| 99-100 | Palatial. The dwelling has `dice: 2d20+5` rooms and is roughly the size of a castle. There’s `dice: 1d8<5` chance that it actually is a castle. There’s an additional `dice: 1d6<4` chance that there are `dice:2d4` outbuildings, with `dice: 4d4` rooms between them. If the structure is not a castle or keep there’s `dice: 1d6<4` chance the buildings are surrounded by walls or similar fortifications.                                                                                 |
^dwellingSize

#### Fortifications

24-table-3.md

| d100   | Result                                                                                                                                                                                                                   |
|:------ |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1-20   | Wall. `dice: [[Fill#^wallstraight]]`, `dice: [[Fill#^walllength]]`, `dice: [[Fill#^wallheight]]`, made of `dice: [[Fill#^wallmaterial]]`. A wall has  `dice: 1d12<2`   magical property (refer to the section on Magic). |
| 21-40  | Hillfort. `dice: [[Fill#^Hillfortsize]]`                                                                                                                                                                                                               |
| 41-55  | Berm. `dice: [[Fill#^bermage]]`, length `dice: [[Fill#^walllength]]`, `dice: [[Fill#^bermshape]]` , `dice: [[Fill#^bermheight]]`, `dice: [[Fill#^bermstructures]]`                                                                                                                                                                                                                 |
| 56-75  | Trench.`dice: [[Fill#^bermage]]`, length `dice: [[Fill#^walllength]]`, `dice: [[Fill#^bermshape]]` , `dice: [[Fill#^bermheight]]`, `dice: [[Fill#^bermstructures]]`, `dice: [[Fill#^trenchhazard]]`                                                                                                                                                                                                                  |
| 76-85  | Tower. It is `dice: [[Fill#^dwellingCondition]]` its age is `dice: [[Fill#^monumentAge]]`, `dice: [[Fill#^TowerMaterial]]`                                                                                                                                                                                                                  |
| 86-95  | Keep. It is `dice: [[Fill#^dwellingCondition]]` its age is `dice: [[Fill#^monumentAge]]` `dice: [[Fill#^TowerMaterial]]`                                                                                                                                                                                                                  |
| 96-100 | Castle. It is `dice: [[Fill#^dwellingCondition]]` its age is `dice: [[Fill#^monumentAge]]` `dice: [[Fill#^TowerMaterial]]`                                                                                                                                                                                                                |
^fortificationType


Just as there are dwellings scattered throughout the wilds there are also countless structures erected primarily for strategic purposes. These structures differ from dwellings in that their primary purpose is to provide a fortified position for the builders, as opposed to living quarters. When possible such structures will be located in areas that provide a wide field of vision of the surroundings.

The age of the fortification will be . . .

[[Fill#^monumentAge]]

It will be in the following condition. Subtract 1 from the roll for every 100 years in age, with a maximum modifier of –15:

[[Fill#^dwellingCondition]]

The fortifications will be built out of the following . . .


24-table-2.md

| d100   | Result                                                                                                                                                                      |
|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-40   | Earth.  Typically  these  will  be  the  simplest kinds of fortifications: earthen berms behind which troops can hide, trenches dug into the earth lined with spikes, etc.  |
| 41-70  | Wood.  The  fortifications  will  be  primarily constructed  of  wood  and  will  be  either  a palisade, a hastily erected wall, a fort framed from massive logs, etc.     |
| 71-90  | Stone. These  could  be  a  stone  wall  snaking across  the  terrain,  a  granite  redoubt  carved into  living  rock  or  a  keep  perched  atop  a lonely tor.           |
| 91-98  | Exotic Material. The defensive structure will be built out of some sort of exotic material, that  may  or  may  not  have  been  created  or crafted through mundane means. |
| 99-100 | Magical Material. The defensive structure is clearly magical in nature: a wall of flame, or corpses, or a castle made from ice.                                             |
^fortificationMaterial


##### Walls
This section covers boundary walls as opposed to walls that would encircle a keep or settlement. A boundary wall demarcates the border between two territories, perhaps that no longer even exist, or was erected to serve as a defensive bulwark during a battle or conflict, then left to remain standing.

Assume that a wall begins in the subhex in which it is rolled for, running north (1), northeast (2), east (3), southeast (4), south (5), southwest (6), west (7), or northwest (8). 

It will be 


| dice: 1d6 | result              |
| --------- | ------------------- |
| 1-3       | relatively straight |
| 4-5       | curved              |
| 6         | sharply angled      |
^wallstraight

How long is the wall?

24-table-1.md

| dice: d100 | Result                                                                                                                                                                                                                                                   |
|:---------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-10       | `dice: 2d20` feet.                                                                                                                                                                                                                                       |
| 11-25      | `dice: 8d20` feet. Walls of this length have `dice: 1d6<3` gate or opening along the length. Berms  this  long  have `dice: 1d6<4` single break somewhere along the line to allow passage.                                                               |
| 26-65      | `dice: 8d100` feet. Walls/Berms of this length have a `dice: 1d6<4`   a  gate  or  opening  every `dice: 1d4`×100 feet. If the wall is taller than 10’  there is `dice: 1d6<2` tower or other defensive structure located every `dice: 1d6`×100 feet.    |
| 66-75      | `dice: 8d100`×10 feet. Walls/Berms of this length have a `dice: 1d6<4`   a  gate  or  opening  every `dice: 1d4`×100 feet. If the wall is taller than 10’  there is `dice: 1d6<2` tower or other defensive structure located every `dice: 1d6`×100 feet. |
| 76-85      | `dice: 1d6` miles. Walls/Berms of this length have a `dice: 1d6<4`   a  gate  or  opening  every `dice: 1d4`×100 feet. If the wall is taller than 10’  there is `dice: 1d6<2` tower or other defensive structure located every `dice: 1d6`×100 feet.     |
| 86-96      | `dice: 3d4` miles. Walls/Berms of this length have a `dice: 1d6<4`   a  gate  or  opening  every `dice: 1d4`×100 feet. If the wall is taller than 10’  there is `dice: 1d6<2` tower or other defensive structure located every `dice: 1d6`×100 feet.     |
| 97-99      | `dice: 5d20` miles. Walls/Berms of this length have a `dice: 1d6<4`   a  gate  or  opening  every `dice: 1d4`×100 feet. If the wall is taller than 10’  there is `dice: 1d6<2` tower or other defensive structure located every `dice: 1d6`×100 feet.    |
| 100        | 100+ miles long. Walls/Berms of this length have a `dice: 1d6<4`   a  gate  or  opening  every `dice: 1d4`×100 feet. If the wall is taller than 10’  there is `dice: 1d6<2` tower or other defensive structure located every `dice: 1d6`×100 feet.       |
^walllength

The wall will be


| dice: 1d216 | result                        |
| ----------- | ----------------------------- |
| 1-72        | `dice: 1d4` feet tall (1-2),  |
| 73-144      | `dice: 2d4` feet tall (3-4),  |
| 144-180     | `dice: 3d4` feet tall (5), or |
| 181-204     | `dice: 4d6` feet tall (6).    |
| 205-212     | `dice: 5d20` feet tall        |
| 213-216     | `dice: 5d100` feet tall       |
^wallheight




Walls are built of 
| dice: 1d12 | result                 |
| ---------- | ---------------------- |
| 1-4        | wood,                  |
| 5-7        | stone,                 |
| 8-10       | brick,                 |
| 11         | an exotic material, or |
| 12         | magic.                 |
^wallmaterial

##### Hillforts
Using the very contours of the land as a defensive feature hillforts tend to be somewhat primitive in nature. Typically, a hill is contoured, with dirt removed to level sections being used to created earthen walls behind which defenders may shelter. Wood and stone can be incorporated into the fort as well, but most times the primary material used is packed dirt.

Most of the time hillforts will be used purely as defensive structures, but over time these will often begin to attract houses and settlements to the relatively safety of the fortifications. If they remain, these hillforts will occasionally be built into larger communities, defended by more sophisticated walls and keeps.

25-table-1.md

| d100   | Result                                                                                                                                                                                                                                                                                                            |
|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-20   | Encompasses  `dice: 1d10`×1,000  sq.  ft.  Has  one “terrace”  with  ramparts  `dice: 1d6+4`  feet  tall  and one entrance.                                                                                                                                                                                                       |
| 21-60  | Encompasses  `dice: 1d100`×1,000  sq.  ft.  Has  one terrace with ramparts `dice: 1d6+6` feet tall and one entrance.                                                                                                                                                                                                              |
| 61-90  | Encompasses  `dice: 1d10`×10,000  sq.  ft.  Has  one terrace  if  under  90,000  sq.  ft.,  two  terraces if over that. The ramparts will be `dice: 1d6+6` feet tall, with `dice: 1d2` entrances per terrace.                                                                                                                             |
| 91-99  | Encompasses `dice: 1d100`×10,000 sq. ft.  Has `dice: 1d2+1`  terraces,  with  ramparts  `dice: 1d8+7`  feet tall, and `dice: 1d3` entrances per terrace.                                                                                                                                                                                          |
| 100    | Encompasses `dice: 3d100`×10,000 sq. ft.  Has `dice: 1d3+1`  terraces,  with  ramparts  `dice: 1d8+7`  feet tall, and `dice: 1d4` entrances per terrace. Hillforts encompassing more than 2,000,000 sq. ft. are largely useless as defensive structures and are instead used  for more pedestrian purposes, such as the containment of livestock. |
^Hillfortsize

##### Berm

Dirt has been dug and piled into a raised fortification, typically as a short-term protective measure. The trench created by the excavation is typically on the outside of the berm, facing the threat, and can be filled with water, or sharpened stakes, or magically summoned oozes, etc.

It will be . .

25-table-4.md

| dice: d100  | Result                                                                                                                                                                                                                                                                                                                                                                                                                         |
|:----- |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1-10  | 1d10 months old for a berm that is fewer than ten years old `diece: 1d6<4` chance it is currently being used;                                                                                                                                                                                                                                                                                                                    |
| 11-60 | 1d10 years old. For a berm that is fewer than ten years old `diece: 1d6<4` chance it is currently being used; Berms that are older than two years, and either not in use or not being well-maintained, will likely be discovered in the process of being taken back over by nature; plants will have begun to reclaim the earthen slopes, trenches get filled in by leaves and decaying  vegetable matter, water, and so forth |
| 61-99 | 10d10 years. For a berm that is older than ten years old `diece: 1d6<2` chance it is currently being used; Berms that are older than two years, and either not in use or not being well-maintained, will likely be discovered in the process of being taken back over by nature; plants will have begun to reclaim the earthen slopes, trenches get filled in by leaves and decaying  vegetable matter, water, and so forth    |
| 100   | 10d100 years. For a berm that is older than ten years old `diece: 1d6<2` chance it is currently being used; Berms that are older than two years, and either not in use or not being well-maintained, will likely be discovered in the process of being taken back over by nature; plants will have begun to reclaim the earthen slopes, trenches get filled in by leaves and decaying  vegetable matter, water, and so forth   |
^bermage

For a berm that is fewer than ten years old there’s a 1-3 in 6 chance that it is currently being used; those older have only a 1 in 6 chance of being in use. As a general rule, older berms have a tendency to be converted over time to actual walls and more defensive permanent structures.

Berms that are older than two years, and either not in use or not being well-maintained, will likely be discovered in the process of being taken back over by nature; plants will have begun to reclaim the earthen slopes, trenches get filled in by leaves and decaying  vegetable matter, water, and so forth. For trenches that are currently being used for defensive purposes refer to the next section, below.

The berm will be 


| dice: 1d8 | result                      |
| --------- | --------------------------- |
| 1-3       | a straight line,            |
| 4-5)      | a curve that is unclosed,   |
| 6-7       | a fully enclosed circle, or |
| 8         | another enclosed shape.     |
^bermshape

It will be this long . . .

[[Fill#^walllength]]

25-table-3.md


| dice: d100   | Result            |
|:-------|:------------------|
| 1-25   | `dice: 1d4+4` feet tall   |
| 26-86  | `dice: 1d6+8` feet tall   |
| 87-99  | `dice: 1d12+12` feet tall |
| 100    | `dice: 1d20+20` feet tall |
^bermheight

Berms are typically as wide at the base as they are tall, sloped more severely on the outside, with a gentler slope on the inside to allow defenders easier access to the top. Berms that are currently being used have a 1 in 6 chance per 8 feet in height of having 


| dice: 1d36 | result                                                                                                   |
| ---------- | -------------------------------------------------------------------------------------------------------- |
| 1-30       | no structures                                                                                            |
| 31-33      | internal structures that allow defenders to reach the top. These structures will be fashioned from earth |
| 34-35      | internal structures that allow defenders to reach the top. These structures will be wood                 |
| 6          | internal structures that allow defenders to reach the top. These structures will be stone.               |
^bermstructures


26-table-1.md

| d100   | Result        |
|:-------|:--------------|
| 1-10   | 1d10 years    |
| 11-60  | 10d10 years   |
| 61-99  | 10d100 years  |
| 100    | 10d1000 years |

##### Trenches
The opposite of berms, trenches are dug into the ground to provide protection to forces or an obstacle to advancing enemies. Use the tables above to determine length and depth. Use the chances given above for gates or openings to determine whether a trench has some means of crossing, such as a bridge. Trenches by themselves have a 

| dice: 1d18 | result                                                                                             |
| ---------- | -------------------------------------------------------------------------------------------- |
| 1-12       | Trench does not contain any hazard in 6 chance of  some sort:                                |
| 13         | containing a hazard of spikes of sharpened wood or iron,                                     |
| 14         | covered and disguised to look like the ground,                                               |
| 15         | containing a hazard of oil or other flammable materials,                                     |
| 16         | containing a hazard of creatures such as giant centipedes, oozes, jellies, etc.              |
| 17         | containing a hazard of undead or animated creatures tasked with attacking those entering, or |
| 18         | containing a hazard of cached boulders or logs primed to roll down the slope.                |
^trenchhazard

If the trenches are more than a year old or abandoned there’s a 1-3 in 6 chance any hazards have been rendered useless by age and the elements. Abandoned trenches also have a 1-2 in 6 chance of being filled with water.


##### Tower/Keep/Castle

[[fill#^monumentAge]]
Subtract 1 from the roll for every 100 years in age, with a maximum modifier of –10:
[[Fill#^dwellingCondition]]

26-table-4.md

| d100   | Result                                                                                                                                         |
|:-------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
| 1-30   | Wood.  The  structures  are  made  of  worked wood,  limiting  their  size  to  no  more  than four stories tall (approximately 50 feet high). |
| 31-80  | Stone. Built primarily of stone, these structures have a size limited to eight stories (approximately 100 feet high).                          |
| 81-100 | Exotic.  Built  from  exotic  materials  or  with the aid of magic, towers may be carved from living trees, or glass.                          |
^TowerMaterial

Towers are typically used as fortified residences or smaller garrisons to secure small areas. However, towers are quick and easy to build and are often implemented as a first “wave” of civilization designed to provide a quick and dirty fortified garrison. Towers have a base value of `dice: 1d12 * 5000` gp.

Keeps are larger, designed to control larger territories, and provide housing and shelter for the settlers. Keeps have a base value of `dice: 3d6 * 10000` gp.

Castles are larger still, the last stage in the evolution of defensive structures. Towers are built to quickly pacify the wilderness, and as civilization spreads they get expanded into keeps, which in turn are added onto and become sprawling castles. Castles have a base value of `dice: 2d6 * 100000` gp, and often house hundreds of residents.

The chance that a structure is uninhabited decreases based upon its size; towers are the most likely to be found uninhabited and castles the least likely. The beginning of this section gives chances that a structure is used for its intended purpose; add 1 to the roll for castles and subtract 1 for towers.

Ex. Structures in Borderlands hexes have a 1-3 in 6 chance of being used for their intended purpose. Towers, therefore, have a 1-2 in 6 chance, keeps a 1-3, and castles a 1-4 chance.

#### Infrastructure

26-table-3.md

| dice: d20 | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|:--------- |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1-8       | Roads `dice: [[Fill#^roadType]]`, There’s `dice: 1d6<5` chance the road follows a nearby terrain feature. If not, roll 1d6 and use the diagram on p., Road Start `dice: [[Fill#^RoadStartEnd]]`, Road End `dice: [[Fill#^RoadStartEnd]]`, The road is . . . `dice: [[Fill^RoadSize]]`. The Road goes on in the `dice: [[Fill#^direction]]` for `dice: [[Fill#^roadlength]]`,The Road goes on in the `dice: [[Fill#^direction]]` for `dice: [[Fill#^roadlength]]`, The road has `dice: [[Fill#^roadmarkers]]`, see [[#Roadcommerce]]  |
| 9-15      | Water. A `dice: [[Fill#^WaterStructureType]]`, dice: `[[Fill#^monumentAge]]`,                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | 
| 16-20     | Commercial `dice: [[Fill#^CommercialType]]`, `dice: [[Fill#^CommercialAbandoned]]`, Inhabited by `dice: [[Fill#^commercialinhabitants]]`, Age: `dice: [[Fill#^monumentAge]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
^InfrastructureType


##### Road

26-table-5.md

| d100   | Result                                                                                                                         |
|:------ |:------------------------------------------------------------------------------------------------------------------------------ |
| 1-30   | Dirt.  Dirt  roads  do  not  grant  the  bonus  to movement  (see  p.  111,  OSE  core)  during rain, or for 1d3–1 days after. |
| 31-60  | Paved with dry laid stones (1-3) or bricks (4-6).                                                                              |
| 61-90  | Wood (logs laid side by side), a “plank road”.                                                                                 |
| 91-98  | Artificial (such as Roman concrete roads).                                                                                     |
| 99-100 | Magical or unusual (see below). `dice: 1d6<2` `dice: [[Fill#^roadunusual]]` `dice: [[Fill#^roadunique]]`                                                   |
^roadType


| dice: 1d6 | result                                                                                |
| --------- | ------------------------------------------------------------------------------- |
| 1-2       | the unusual aspect of the road can be found the entire length of the road, on a |
| 3-4       | it is found for `dice: 1d8`×10% of the length, and on a                         |
| 5-6       | it occurs only in a single randomly determined location.                        |
^roadunusual

27-table-1.md

| d10  | Result                                                                                                                                                |
|:---- |:----------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-3  | Unique material. The road is built of an unusual material. The road is made from `dice: [[Fill#^roadmaterialunusual]]`                                |
| 4-6  | Unique construction. The road is built in an unusual manner. It is `dice: [[Fill#^roadconstructionunusual]]`                                          |
| 7    | Magical (benign). The road is enchanted in a manner that is beneficial to those traveling on it. It `dice: [[Fill#^roadmagicbenign]]`                  |
| 8    | Magical (malign). The road is enchanted in a manner that is dangerous to those traveling on it. `dice: [[Fill#^roadmagicmalign]]`                     |
| 9-10 | Magical  (neutral).  The  road  possesses  an enchantment that is neither directly beneficial nor malignant. It is `dice: [[Fill#^roadmagicneutral]]` |
^roadunique


| dice: 1d10 |                                                               |
| ---------- | ------------------------------------------------------------- |
| 1          | one of the materials above, but unique or rare to the region, |
| 2          | iron,                                                         |
| 3          | bone,                                                         |
| 4          | graves,                                                       |
| 5          | glass,                                                        |
| 6          | high-tech material like plastic or concrete,                  |
| 7          | ceramics,                                                     |
| 8          | living material,                                              |
| 9-10       | other.                                                        |
^roadmaterialunusual

| dice: 1d6 | result                          |
| --------- | ------------------------------- |
| 1         | elevated,                       |
| 2         | sunken,                         |
| 3         | covered,                        |
| 4         | hidden,                         |
| 5         | goes underground for a portion, |
| 6         | other.                          |
^roadconstructionunusual

| dice. 1d8 |                                                                                                                                                                |
| --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1         | is safer than normal. Wandering monster chances are reduced by 1d2 while on the road,                                                                          |
| 2         | those on the road are under the effects of a permanent protection from evil spell,                                                                             |
| 3         | food does not spoil or go bad while on the road,                                                                                                               |
| 4         | travelers on the road move faster than normal: if granted, the normal 50% bonus to movement is increased to 75%, or if not granted travelers have a 25% bonus, |
| 5         | travelers on the road do not incur exhaustion for forced marching,                                                                                             |
| 6         | healing is increased: roll twice for all healing spells and effects and take the better of two results,                                                        |
| 7         | all travelers on the road are able to understand any spoken language, or                                                                                       |
| 8         | other.                                                                                                                                                         |
^roadmagicbenign

| dice: 1d8 |                                                                                                                                    |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| 1         | It is more dangerous than normal: those traveling on the road have their chances of wandering monsters increased by 1d2,           |
| 2         | normal rations spoil after a day on the road and iron rations after 1d4 days,                                                      |
| 3         | movement is slowed: if a speed bonus would normally be granted for maintained roads it is lost, and if not movement is 50% slower, |
| 4         | turning undead is less potent: if attempting to turn undead within 50’ of the road roll twice, taking the lower result,            |
| 5         | sleep within 50’ of the road is fitful, and does not count as rest for purposes of memorizing spells or avoiding exhaustion,       |
| 6         | healing magics are minimized: roll twice when determining damage healed, taking the lower of the two results,                      |
| 7         | creatures slain on the road are either , `dice: [[Fill#^roadslain]]`                                                                |
| 8         | other.                                                                                                                             |
^roadmagicmalign


| dice: |                                                                                                                                                                                                                                                       |
| ----- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1     | a pathway to , `dice: [[Fill#^roadpathway]]`                                                                                                                                                                                                          |
| 2     | can  only  be  traveled  on  by  those  who  `dice: [[Fill#^roadAccess]]`                                                                                                                                                                             |
| 3     | the  road  is  lit  by  floating magical  lights:  there’s  `dice: 1d6<3` chance  the lights  only  illuminate  when  living  creatures are within 30’, otherwise they stay lit,                                                                      |
| 4     | the road is intelligent, inhabited by an animating spirit;  it  is  `dice: [[Fill^alignment]]`; the road has an Intelligence of `dice: 3d6`, and there’s  `dice: 1d6<3` chance it has properties similar to an intelligent sword see p. 272 OSE core, |
| 5     | the road only appears under certain conditions or at certain times of the year refer to the Magic Chapter on p. 66,  or                                                                                                                               |
| 6     | other.                                                                                                                                                                                                                                                |
^roadmagicneutral

| dice. 1d6 | result                      |
| --------- | --------------------------- |
| 1-4       | another place  (1-4)  or    |
| 5-6       | plane  of  existence  (5-6) |
^roadpathway

| dice: 1d6 |                                       |
| --------- | ------------------------------------- |
| 1-3       | know the  proper  words  (1-3)         |
| 4-6       | or  carry  the  correct charms  (4-6) |
^roadAccess

| dice: 1d8 | result       |
| --------- | ------------ |
| 1-2       | Lawful,      |
| 3-6       | Neutral,  or |
| 7-8       | Chaotic      |
^alignment


| dice: 1d6 |                                                                                              |
| --------- | -------------------------------------------------------------------------------------------- |
| 1-2       | incapable of being raised or brought back to life, short of a wish spell, or                 |
| 3-6       | raised as undead within 1d8 days of their death; they will be `dice: [[Fill#^TypePCUndead]]` |
^roadslain

| dice: 1d6 | result     |
| --------- | ---------- |
| 1-2       | skeletons, |
| 3-4       | zombies,   |
| 5         | wights, or |
| 6         | wraiths    |
^TypePCUndead

Magical enchantments can 

| dice: 1d6 |                                                                                         |
| --------- | --------------------------------------------------------------------------------------- |
| 1         | be dispelled by conducting a ritual that needs to be researched,                        |
| 2         | be dispelled by a casting of dispel magic by a caster of level `dice: 1d6+8` or higher, |
| 3         | be dispelled by a casting of remove curse by a caster of at least level 1d6+8,          |
| 4         | be dispelled, but only for `dice:1d12` months by one of the above methods, or           |
| 5-6       | not be dispelled by anything short of divine intervention.                              |
^roaddispel

Magical effects that stretch for more than one mile: `dice: 1d6<4` will require multiple attempts to dispel on a roll of 

There’s `dice: 1d6<5` chance the road follows a nearby terrain feature. If not, roll 1d6 and use the diagram on p.

The road starts or stops in this hex? `dice: 1d6<3`. Otherwise, it is assumed the road passes through the hex.

The road leads to (roll twice, once for each end. If the road terminates in the current hex assume it leads to the most appropriate feature) . . .

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
^RoadStartEnd

##### Roadcommerce
In Borderland hexes the road has  `dice: 1d6<5` chance of being used regularly for commerce and travel. This chance is increased by one in Civilized hexes and decreased by 1 in Wilderness hexes, or domains with an alignment of Chaotic. Roads that are not used regularly have fallen into disrepair and do not grant the 50% bonus to overland movement (see p. 111, OSE core).
If a road connects two settlements, add the highest Market Class to the following roll for the size of the road. Refer to p. 16 of Domain Building for information on Market Classes.

#####

The road is . . .

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
^roadsize


Add +5 to the above roll in Civilized domains, and an additional +5 if the domain is Lawful or advanced (either magically or technologically).

There’s a base 1-2 in 6 chance the road has 

| dice: 1d18 | result                                                                                                                           |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 1-12       | no markers                                                                                                                       |
| 13-15      | markers that indicate communities that lie along the road,                                                                       |
| 16- 17     | distance markers that divide the road into equal increments, or                                                                  |
| 18         | both markers that indicate communities that lie along the road and distance markers that divide the road into equal increments . |
^roadmarkers

When rolling to determine the length of the road you will roll either once (if the road terminates in the chosen hex) or twice (if the road passes through the hex). If rolling once take the result and double it. If rolling twice add the two numbers together to get the total length of the road. When rolling twice designate which roll is for which length of road exiting the hex.


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
^roadlength

Roads that cross a river have a base 1-2 in 6 chance of crossing at a bridge. Subtract 1 from the chance in Wilderness hexes, add 1 in Civilized hexes, and add 1 if the road is a lane or 2 if it is a road (see above). Refer to p. 26 to determine the type of bridge.


North
North East
East 
South-East
South
South-West
West
North-West
^direction

##### Water

Features in this category include man-made means of controlling or accessing water. This includes aqueducts and wells, canals, irrigation ditches, man-made lakes and ponds, etc.

The water feature’s age is . . .

28-table-2.md

| d100   | Result        |
|:-------|:--------------|
| 1-10   | 1d10 years    |
| 11-60  | 10d10 years   |
| 61-99  | 10d100 years  |
| 100    | 10d1000 years |
^WaterstructureAge


There’s a 1-3 in 6 chance that a water feature is currently in use. This chance decreases by 1 in Wilderness hexes and/or if the feature is over 500 years old and increases by 1 if in Civilized hexes and/or it is less than one hundred years old (for a total range of modifiers of –2 to +2).

A feature that is not currently in use will typically have fallen into disrepair or could potentially serve as a lair for dangerous creatures that prevent its use.

The feature is . . .

29-table-1.md

| d100  | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|:----- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 01-05 | Aqueduct, `dice: [[Fill#^Aqueductheight]]`, `dice: [[Fill#^Aqueductlength]]`, `dice: [[Fill#^Aqueductmaterial]]` There’s  `dice: 1d6<5` chance the aqueduct supports will be of the same material as the channel itself. If not, roll again to determine what the supports are made of. It will be `dice: [[Fill#^aqueductopen]]`, supported by  pillars]]`,                                                                                                                                                                                                                                                                                                                                                                                  |
| 06-40 | Bridge There’s `dice: 1d20` chance that the waterway has dried up or moved location, and `dice: 1d20` chance that the road that once ran over the bridge no longer exists, or perhaps never did.Length `dice: [[Fill#^bridgelength]]`, width `dice: [[Fill#^bridgewidth]]`material `dice: [[Fill#^bridgematerial]]`, There’s a `dice: 1d6<5` chance the bridge is in use and safe to cross. This is increased by 1 in Civilized hexes, and reduced by 1 in Wilderness hexes. Bridges that are not safe to cross are either `dice: [[Fill#^bridgeUnsafe]]`                                                                                                                                                                                     |
| 41-45 | Canal. Purpose: `dice: [[Fill#^CanalPurpose]]`, There is `dice: 1d6<5` chance that a canal is being used for its intended purpose. This chance is increased by 1 in Civilized hexes and reduced by 1 in Wilderness hexes. Canals that are not being used have a 1 in 6 chance of being permanently empty. length `dice: [[Fill#^Canallength]]`, width `dice: [[Fill#^Canalwidth]]`, depth: `dice: [[Fill#^Canalwidth]]`. It is `dice: [[Fill#^Constantlyfilled]]`                                                                                                                                                                                                                                                                             |
| 46-55 | Fountain. Made of `dice: [[Fill#^fountainMaterial]]`, `dice: [[Fill#^FountainStatue]]`, `dice: [[Fill#^FountainwaterMagical]]` , `dice: [[Fill#^FountainDispel]]`, `dice: [[Fill#^fountainShape]]`. It is `dice: 1d20` feet in diameter, and there’s  `dice: 1d6<2` chance it is flush with the ground.  There’s `dice: 1d6<3` chance a fountain is no longer working, and if that’s the case there’s `dice: 1d6<2` further chance it is empty. There’s `dice: 1d6<2` chance a fountain has the potential to contain a monster, treasure, or trap. If this is the case roll on the Dungeon Stocking Table found on p. 225 of the OSE core rules. If something is present assume the fountain has a “dungeon level” equivalent to `dice: 1d6`. |
| 56-65 | Pond                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 66-00 | Well Wells are drilled or dug into the earth to provide access to water or potentially other liquids.  `dice: [[Fill#^WellotherWater]]`, `dice: [[Fill#^WellDugBy]]`, `dice: [[Fill#^welllinedwith]]`, `dice: [[Fill#^WellWidth]]`, `dice: [[Fill#^Welldepth]]`,  `dice: [[Fill#^wellStructureMaterial]]`, Water is brought to the surface by means of a `dice: [[Fill#^WellMechanics]]` ,  The well is `dice: [[Fill#^WellOk]]`, Magical? `dice: [[Fill#^FountainwaterMagical]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | 
^WaterStructureType



###### Aqueduct

Specifically, raised, artificial channels, pipes, or troughs that carry water from one location to another, often over great distances.

An aqueduct will average . . .


29-table-2.md

| d100   | Result         |
|:-------|:---------------|
| 1-10   | `dice: 3d6` feet tall  |
| 11-50  | `dice: 4d8` feet tall  |
| 51-90  | `dice: 5d10` feet tall |
| 91-100 | `dice: 6d20` feet tall |
^Aqueductheight

29-table-5.md

| d100   | Result                                                                       |
|:-------|:-----------------------------------------------------------------------------|
| 1      | `dice: 5d20` feet long (perhaps this is all that remains of a once elaborate system) |
| 2-5    | `dice: 10d100` feet long                                                             |
| 6-50   | `dice: 1d4` miles long                                                               |
| 51-75  | `dice: 3d6` miles long                                                               |
| 76-99  | `dice: 5d20` miles long                                                              |
| 100    | `dice: 10d100` miles long                                                            |
^Aqueductlength


It will be `dice: 1d12` feet wide.

The aqueduct will be built using . . .

29-table-6.md

| d100   | Result                                                                    |
|:-------|:--------------------------------------------------------------------------|
| 1-5    | Channel created by hollow logs.                                           |
| 6-30   | Brick. Laid and mortared bricks.                                          |
| 31-65  | Clay.                                                                     |
| 66-90  | Stone.                                                                    |
| 91-99  | Metal. Lead, most likely.                                                 |
| 100    | Exotic Materials. Hollow bones, blown glass, magically shaped stone, etc. |
^Aqueductmaterial


There’s  `dice: 1d6<5` chance the aqueduct supports will be of the same material as the channel itself. If not, roll again to determine what the supports are made of.

It will be

| dice: 1d6 |                                 |
| --------- | ------------------------------- |
| 1-4       | open to the sky or              |
| 5-6       | enclosed, and it will either be |
^aqueductopen

supported by 

| dice: 1d6 |                               |
| --------- | ----------------------------- |
| 1-5       | columns or pillars (1-5) or a |
| 6         | solid wall (6). there’s a chance that `dice: [[Fill#^aqueductwall]]` will be incorporated into the design..              |
^aqueductpillars

If it is solid wall there’s a chance that 

| dice: 1d6 |                            |
| --------- | -------------------------- |
| 1-3       | gates,                     |
| 4         | defensive features,        |
| 5         | secret rooms refer to the section on [[#Monuments:]]  to determine if there is anything inside.           |
| 6         | nothing, it is just solid, |
^aqueductwall



###### Bridge

Bridges typically cross rivers or waterways. There’s `dice 1d20` chance that the waterway has dried up or moved location, and `dice 1d20` chance that the road that once ran over the bridge no longer exists, or perhaps never did.



Bridges have an overall length of . . .



29-table-3.md

| dice: d100 | Result             |
|:---------- |:------------------ |
| 1-10       | `dice: 3d6` feet    |
| 11-40      | `dice: 4d10` feet   |
| 41-75      | `dice: 5d20` feet   |
| 76-99      | `dice: 10d100` feet |
| 100        | `dice: 1d4` miles   |
^bridgelength





29-table-4.md

| dice: d100 | Result               |
|:---------- |:-------------------- |
| 1-30       | `dice: 3d4` feet wide. |
| 31-90      | `dice: 5d6` feet wide.       |
| 91-100     | `dice: 6d8` feet wide.       |
^bridgewidth



`dice: [[Fill#^bridgewidth]]`

The bridge will be made out of . . .


29-table-7.md

| d100  | Result                                                                                                                                                              |
|:----- |:------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-10  | Vines or ropes.                                                                                                                                                     |
| 11-30 | Wood. There’s `dice: 1d20<2` chance that the bridge is movable or a drawbridge.                                                                                     |
| 31-60 | Brick. Laid and mortared bricks, potentially plastered.                                                                                                             |
| 61-90 | Stone.                                                                                                                                                              |
| 91-94 | Naturally occurring, carved from the landscape by the elements.                                                                                                     |
| 95-97 | Metal. Iron or steel.                                                                                                                                               |
| 98-99 | Exotic Materials. Hollow bones, blown glass, magically shaped stone, etc.                                                                                           |
| 100   | Magical. `dice: [[Fill#^bridgemagicalmaster]]`. Avoiding or undoing magical effects imparted by crossing a bridge can be achieved by `dice: [[Fill#^BridgeDispel]]` |
^bridgematerial

If the result is Magical roll again to determine the material the bridge is made from (if not a magical substance) after rolling below to determine the nature of the enchantment. Bridges are inherently transitive in nature, taking one from one side to another. The magical nature is 


| dice: 1d6 |  results                                                                                                                                                      |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1-2       | in the bridge’s structure. It is `dice: [[Fill#^bridgeMagicalStructure]]`                                                                              |
| 3-4       | affects those who use the bridge. Crossing the bridge:  `dice: [[Fill#^bridgemagicalCrossing]]`                                                        |
| 5-6       | can only be accessed by those who know the proper words or rituals. If a specific trigger is needed it will be: `dice: [[Fill#^bridgeMagicalTrigger]]` |
^bridgemagicalmaster



If the magical nature is in the bridge it is 


| dice: 1d6 |                                                     |
| --------- | --------------------------------------------------- |
| 1         | invisible,                                          |
| 2         | made of bound wind, flame, water, or other element, |
| 3         | physics-defying,                                    |
| 4         | made of living material,                            |
| 5         | not fastened to anything, or moving,                |
| 6         | other.                                              |
^bridgeMagicalStructure



| dice: 1d6 | result                                                                                                     |
| --------- | ---------------------------------------------------------------------------------------------------- |
| 1         | `dice: [[Fill#^bridgeSpellAges]]`                                                                    |
| 2         | `dice: [[Fill#^bridgeSpellHeal]]`                                                                    |
| 3         | transports the traveler to another plane of existence,                                               |
| 4         | transports the traveler to another place in the same plane,                                          |
| 5         | reverses the traveler’s alignment if they fail a Save v. Spells (Neutral characters are unaffected), |
| 6         | other.                                                                                               |
^bridgemagicalCrossing

| dice: 1d6 |                            |
| --------- | -------------------------- |
| 1-3       | those who cross the bridge age  `dice: 1d12` years,   |
| 4-6       | those who cross the bridge de-age `dice: 1d12` years, |
^bridgeSpellAges


| dice: 1d6 |       |
| --------- | ----- |
| 1-3       | heals those who cross it for 1d12 points of damage |
| 4- 6      | harms those who cross it for 1d12 points of damage |
^bridgeSpellHeal






| dice: 1d8 |                                                                                 |
| --------- | ------------------------------------------------------------------------------- |
| 1         | a specific word or ritual to be spoken before crossing,                         |
| 2         | a specific physical ritual such as closing one’s eyes, walking backwards, etc., |
| 3         | crossing at a specific time,                                                    |
| 4         | a specific object carried with the traveler,                                    |
| 5         | the traveler must be accompanied by a specific individual,                      |
| 6         | a specific payment `dice: [[Fill#^BridgemagicPayment]]`                         |
| 7         | a specific guardian must be defeated, or                                        |
| 8         | other.                                                                          |
^bridgeMagicalTrigger


| dice: 1d6 |             |
| --------- | ----------- |
| 1-2       | monetary,   |
| 3-4       | object,     |
| 5         | service, or |
| 6         | quality),   |
^BridgemagicPayment


 

| dice: 1d6 | result                                                                                      |
| --------- | ------------------------------------------------------------------------------------------- |
| 1         | nothing short of a wish spell or deific intervention,                                       |
| 2         | a remove curse cast by a spellcaster of level `dice: 1d6+8` or greater,                     |
| 3         | a dispel magic cast by a spellcaster of at least level `dice: 1d6+8`,                       |
| 4         | a quest or specific action one undertakes,                                                  |
| 5         | walking backwards across the bridge in the opposite direction it was originally crossed, or |
| 6         | other.                                                                                      |
^BridgeDispel

There’s a `dice: 1d6<5` chance the bridge is in use and safe to cross. This is increased by 1 in Civilized hexes, and reduced by 1 in Wilderness hexes. Bridges that are not safe to cross are either `dice: [[Fill#^bridgeUnsafe]]`

| dice: 1d6 | result                |
| --------- | --------------------- |
| 1-4       | structurally unsound  |
| 5-6       | inhabited by monsters |
^bridgeUnsafe


###### Canal

Artificial waterways that channel water for irrigation, drainage, or transportation, canals will be 

| dice: 1d6 |                                                                                       |
| --------- | ------------------------------------------------------------------------------------- |
| 1-3       | constantly filled with water. It is `dice: [[Fill#^CanalReasonConstantlyFilled]]`     |
| 4-6       | only filled when in use or only usable when filled.  `dice: [[Fill#^CanalHowFilled]]` |
^Constantlyfilled

Canals that are not always filled will either be 

| dice: 1d6 |                                                                           |
| --------- | ------------------------------------------------------------------------- |
| 1-2       | manually filled  `dice: [[Fill#^CanalManuallyFilled]]`                    |
| 3-6       | filled naturally. Canals that are naturally filled either                 |
| 1-3       | rely on rain, filling for `dice: 1d4` inches per day of rainfall or       |
| 4-6       | rely on seasonal weather (such as glacial melt, or the rainy season, etc. |
^CanalHowFilled

| dice: 1d6 |                                                                  |
| --------- | ---------------------------------------------------------------- |
| 1-4       | connected to a nearby source of water such as a lake or river or |
| 5-6       | filled through magical or other means.                           |
^CanalReasonConstantlyFilled

| dice: 1d6 |               |     |
| --------- | ------------- | --- |
| 1-4       | mechanical or |     |
| 5-6       | magical means | or  |
^CanalManuallyFilled


Canals 

| dice: 1d6 |                                                     |
| --------- | --------------------------------------------------- |
| 1-3       | provide water to dry areas,                         |
| 4-5       | remove water from wet areas, or                     |
| 6         | are used for the transportation of goods or people. |
^CanalPurpose

Canals that are always filled will be 



A canal will be . . .


30-table-1.md

| d100   | Result              |
|:-------|:--------------------|
| 1-5    | `dice: 10d20` feet long     |
| 6-30   | `dice: 10d100` feet long    |
| 31-50  | `dice: 1d4` miles long      |
| 51-75  | `dice: 1d12` miles long     |
| 76-97  | `dice: 5d20` feet wide/deep |
| 98-100 | `dice: 10d100` miles long   |
^Canallength


It is (roll separately for width/depth) . . .

30-table-2.md

| d100   | Result              |
|:-------|:--------------------|
| 1-10   | `dice: 1d4` feet wide/deep  |
| 11-35  | `dice: 2d6` feet wide/deep  |
| 36-65  | `dice: 3d8` feet wide/deep  |
| 66-90  | `dice: 4d10` feet wide/deep |
| 91-100 | `dice: 5d12` feet wide/deep |
^Canalwidth


There is `dice: 1d6<5` chance that a canal is being used for its intended purpose. This chance is increased by 1 in Civilized hexes and reduced by 1 in Wilderness hexes. Canals that are not being used have a 1 in 6 chance of being permanently empty. 



###### Fountain

A fountain serves both decorative and functional purposes. In both cases, they are most often created using naturally occurring underground springs where there is enough water pressure to bring the water above ground level.

Fountains are artificially created by using impermeable substances to fashion bowl-shaped depressions, which are often surrounded by a low border and can also include statuary mounted inside from which the water emerges.

The fountain will be made from . . .

31-table-1.md

| d100   | Result                                                                                                         |
|:-------|:---------------------------------------------------------------------------------------------------------------|
| 1-5    | Wood.                                                                                                          |
| 6-40   | Brick. Often coated in plaster or adobe.                                                                       |
| 41-95  | Stone. (1-4) fitted and mortared stone or (5-6) carved from stone.                                             |
| 96-99  | Exotic Material. Bone, petrified wood, living trees, etc.                                                      |
| 100    | Magical.  The fountain is fashioned from magical materials such as never-melting ice, an enormous flower, etc. |
^fountainMaterial

Fountains have a

1-4 in 6 chance of incorporating statuary into the design. 


| dice: 1d6 |                                                            |
| --------- | ---------------------------------------------------------- |
| 1-4       | There are Statues `dice: [[Fill#^FountainMagicalStatues]]` |
| 5-6       |                                                            |
^FountainStatue

| dice: 1d12 |                                                                     |
| ---------- | ------------------------------------------------------------------- |
| 1          | the statuary is magical `dice: [[Fill#^FountainTypemagicalStatue]]` |
| 2-12       |                                                                     |
^FountainMagicalStatues


There’s a 1 in 12 chance that the statuary is magical. It 

| dice: 1d6 |                                                                                                                         |                       |      |
| --------- | ----------------------------------------------------------------------------------------------------------------------- | --------------------- | ---- |
| 1         | is a guardian that attacks those who attempt to drink without a proper offering (use stats of a crystal living statue), |                       |      |
| 2         | will offer cryptic advice to those who drink from it,                                                                   |                       |      |
| 3         | will stare wordlessly at those who approach but do no harm,                                                             |                       |      |
| 4         | moves, but only when no one is looking,                                                                                 |                       |      |
| 5         | assumes the form of the first person who drinks from it and seeks to replace them                                       | treat as doppelganger | , or |
| 6         | other.                                                                                                                  |                       |      |
^FountainTypemagicalStatue





| dice: 1d20 |                                                     |
| ---------- | --------------------------------------------------- |
| 1          | The water within the fountain/well possesses a magical dweomer. `dice: [[Fill#^FountainDweomer]]`, `dice: [[Fill#^FountainwaterPlace]]`, `dice: [[Fill#^FountainWaterTime]]` |
| 2-20       |                                                     |
^FountainwaterMagical


| dice: 1d12 |                                                                            |
| ---------- | -------------------------------------------------------------------------- |
| 1          | This magic lasts for long once removed from the source. Those drinking from the water |
| 2-12       | magic only short duration                                                  |
^FountainwaterPlace




| dice: 1d6 |                                                                                                                          |
| --------- | ------------------------------------------------------------------------------------------------------------------------ |
| 1         | `dice: [[Fill#^fountainhealharm]]`                                                                                       |
| 2         | `dice: [[Fill#^fountainsaveDie]]`                                                                                        |
| 3         | `dice: [[Fill#^FountainBuff]`                                                                                            |
| 4         | `dice: [[Fill#^fountainBonus]]`                                                                                          |
| 5         | are brought back to life if submerged in the pool, provided they have not been dead for more than `dice: 1d12` hours, or |
| 6         | other.                                                                                                                   |
^FountainDweomer

| dice: 1d6 |                         |
| --------- | ----------------------- |
| 1-3       | are healed for `dice: 1d6+1` hp |
| 4-6       | or harmed for `dice: 1d6+1` hp  |
^fountainhealharm


| dice: 1d6 |                               |
| --------- | ----------------------------- |
| 1-3       | are cured of all damage       |
| 4-6       | or must Save v. Poison or die |
^fountainsaveDie


| dice: 1d6 |                                                   |
| --------- | ------------------------------------------------- |
| 1-3       | increase                                          |
| 4-6       | or decrease a random ability score by 1d4 points, |
^FountainBuff



| dice: 1d6 |                                      |
| --------- | ------------------------------------ |
| 1-3       | gain a +1d4 bonus to their next roll |
| 4-6       | or subtract the same                 |
^fountainBonus

| dice: 1d6 |                                                        |
| --------- | ------------------------------------------------------ |
| 1-4       | The effect of magical water is  permanent or           |
| 5-6       | The effect of magical water lasts for `dice: 1d8` day. |
^FountainWaterTime

Effects can only be removed by

| dice: 1d6 |                                                                    |
| --------- | ------------------------------------------------------------------ |
| 1         | a wish or divine intervention,                                     |
| 2         | a remove curse cast by a spellcaster of level 1d6+8 or greater,    |
| 3         | a dispel magic cast by a spellcaster of at least level 1d6+8,      |
| 4         | accepting a geas from the spirit that resides within the fountain, |
| 5         | making the appropriate offering to the fountain, or                |
| 6         | other.                                                             |
^FountainDispel

 

| dice: 1d6 |                                                             |
| --------- | ----------------------------------------------------------- |
| 1-3       | The fountain is round,                                      |
| 4-5       | The fountain is rectangular, or                             |
| 6         | The fountain is not round or rectangular but another shape. |
^fountainShape

It is `dice: 1d20` feet in diameter, and there’s  `dice: 1d6<2` chance it is flush with the ground.  There’s `dice: 1d6<3` chance a fountain is no longer working, and if that’s the case there’s `dice: 1d6<2` further chance it is empty. There’s `dice: 1d6<2` chance a fountain has the potential to contain a monster, treasure, or trap. If this is the case roll on the Dungeon Stocking Table found on p. 225 of the OSE core rules. If something is present assume the fountain has a “dungeon level” equivalent to `dice: 1d6`.

###### Pond

This category assumes the pond is an artificial feature created by an intelligent race damming a river, stream, or other source of water to create a still body of water that can be used for some|purpose. Refer to p. 63 for more information on ponds.

###### Well

Wells are drilled or dug into the earth to provide access to water or potentially other liquids.  `dice: [[Fill#^WellotherWater]]`


| dice: 1d100 |                                                                                             |     |
| ----------- | ------------------------------------------------------------------------------------------- | --- |
| 1           | well has been dug to extract something other than water, `dice: [[Fill#^wellnotWaterWhat]]` |     |
| 2-100       |                                                                                             |     |
^WellotherWater



| dice: 1d6 |                |                                                                         |
| ----------- | ---------------------------------------------------------------------------------------- |
| 1-2         | oil or similar,                                                                          |
| 3-4         | an appropriate fantasy liquid, perhaps magma, or rockmilk (from Mieville’s The Scar|, or |
| 5-6         | magical energy.                                                                          |
^wellnotWaterWhat



Wells are usually 

| dice: 1d20 |                                                                                                        |
| ---------- | ------------------------------------------------------------------------------------------------------ |
| 1-19       | dug by hand,Wells that are dug by hand tend to be fairly wide and not too deep.                                                                                            |
| 20         | dug by other means (magic, or controlled burrowing animals, or technology| can be any width and depth. |
^WellDugBy

and lined with 

| dice: d6 |                                |
| -------- | ------------------------------ |
| 1        | lined with  wood,              |
| 2-3      | lined with  brick,             |
| 4-5      | lined with  stone              | 
| 6        | lined with  another substance. |
^welllinedwith


A well will be . . .

31-table-2.md

| dice: d100   | Result        |
|:-------|:--------------|
| 1-15   | `dice: 1d4` feet wide |
| 16-50  | `dice: 2d4` feet wide |
| 51-85  | `dice: 3d4` feet wide |
| 86-100 | `dice: 4d4` feet wide |
^WellWidth

32-table-1.md

| dice: 100   | Result           |
|:-------|:-----------------|
| 1-15   | `dice: 2d10` feet deep   |
| 16-50  | `dice: 5d12` feet deep   |
| 51-85  | `dice: 10d20` feet deep  |
| 86-99  | `dice: 20d100` feet deep |
| 100    | `dice: 1d4` miles deep   |
^Welldepth

Above-ground wells are typically surrounded by a structure that rises above the surface for three or four feet, often with a roof or overhead covering to prevent contamination by the elements. This structure will be built of . . .

32-table-2.md

| dice: d100   | Result          |
|:-------|:----------------|
| 1-20   | Wood            |
| 21-60  | Brick           |
| 61-90  | Stone           |
| 91-98  | Metal           |
| 99-100 | Exotic material |
^wellStructureMaterial



32-table-3.md

| dice: d100 | Result                                                                                         |
|:---------- |:---------------------------------------------------------------------------------------------- |
| 1-10       | Dipper that is reached into the well.                                                          |
| 11-60      | Bucket on a rope.                                                                              |
| 61-70      | Mechanical screw. `dice: [[Fill#^MechanicalScrew]]`                                                                             |
| 71-85      | Mechanical pump and bladder A pump and bladder is similar to an old-fashioned farm-style pump. |
| 86-99      | Wind turbine. wind turbines resemble those in Western movies.                                  |
| 100        | Magical means. `dice: [[Fill#^WellMagical]]`                                                                                |
^WellMechanics

If the well is deeper than 5 feet add 10 to the above roll.



Mechanical screws could be like an Archimedean screw or a mean| of raising and lowering buckets via pulley. Such devices are 

| dice: 1d6 |                                                                                |
| --------- | ------------------------------------------------------------------------------ |
| 1-3       | powered by an outside force such as a wheel turned by oxen, undead, or slaves, |
| 4-5       | powered by the user, or                                                        |
| 6         | powered by magical means.                                                      |
^MechanicalScrew


Water can also be forced to the surface by magical means, 

| dice: 1d6 |                                             |
| --------- | ------------------------------------------- |
| 1-2       | by a specific spell,                        |
| 3-4       | by a creature bound to perform t|e task, or |
| 5-6       | by a permanent magical item.                |
^WellMagical



| dice: 1d20 |                              |
| ---------- | ---------------------------- |
| 1          | `dice: [[Fill#^WellFouled]]` |
| 2-20       |                              |
^WellOk

| dice: 1d6 |                                                                                                      |
| --------- | ---------------------------------------------------------------------------------------------------- |
| 1-5       | dry and no longer a source of water or                                                               |
| 6         | fouled and no longer potable. Those drinking from a fouled well must `dice: [[Fill#^WellPoisonous]]` |
^WellFouled




| dice: 1d6 |                                                                                                          |
| --------- | -------------------------------------------------------------------------------------------------------- |
| 1-3       | Save v. Poison or suffer the effects of giant centipede poison that lasts for `dice: 1d4` days p. 147, OSE core, |
| 4-5       | Save v. Poison or suffer `dice: 1d12` points of damage, or                                                       |
| 6         | Save v. Poison or die in `dice: 1d6` hours.                                                                      |
^WellPoisonous

Each well has a 1 in 20 chance of possessing an unusual quality. Roll on the fountain magical dweomer table.  [[Fill#^FountainwaterMagical]]

##### Commercial Infrastructure

This section includes those enterprises and businesses typically found outside of an urban settlement. It does not include businesses that are typically found inside cities, although the Referee is certainly welcome to include such infrastructure in the wilderness should it make sense.


32-table-4.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|:------ |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1-5    | Camp `dice: [[Fill#^CampOccupied]]`,Camps have a `dice: 1d6<5` chance of having low defensive walls surrounding the perimeter (`dice: 1d4+2` feet tall).  There is also `dice: 1d6<3` chance someone has been nice enough to keep a stock of dry firewood.  `dice: 1d6<2` camps have semi-permanent, crude shelters for animals or Man. `dice: [[Fill#^campwatersource]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| 6-15   | Farm Size: `dice: [[Fill#^FarmSize]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| 16-17  | Ferry `dice: [[Fill#^ferryoperator]]`, `dice: [[Fill#^ferryfee]]`, `dice: [[Fill#^Ferrycapacity]]` ,`dice: [[Fill#^dishonestferryman]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 18-20  | Ford There’s `dice: 1d6<3` chance that the crossing is dangerous during certain times of the year, or after heavy rain, Fords are `dice: [[Fill#^fordmanmade]]`, Depth: `dice: [[Fill#^forddepth]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 21-25  | Hunting Lodge `dice: [[Fill#^LodgeOwner]]`Hunting lodges consist of `dice: 1d4` buildings, typically, either of `dice: [[Fill#^LodgeMaterial]]` ,Because they are often forced to rely on their own supplies for long periods of time there’s `dice: 1d6<3` chance that a hunting lodge has a Market Class of 1.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| 26-30  | Inn `dice: 1d8[[Fill#^innFeature]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 31     | Lighthouse.Tall buildings with a light atop to  `dice: [[Fill#^Signatower]]`. The towers will be `dice: 3d6*10` feet high and manned by `dice: 1d4` staff with a `dice: 1d6<=4` chance of having `dice: 2d4` mercenary guards.  The fire is `dice: [[Fill#^WhenOn]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| 32-35  | Logging Camp. When found in wooded areas such a camp is dedicated to cutting timber; when found in non-wooded areas the workers harvest sod, peat, or similar material. An ocean-side camp may harvest kelp or something similar. The camp will `dice: [[Fill#^LoggingConnections]]`, Refer to the Resource section on p. 37 to determine the value/size of nearby resources. There will be `dice: 1d6` individuals dedicated to harvesting the material for every subhex of resource. Camps will be `dice: [[Fill#^LoggingPermanent]]`, There will be `dice: 1d2` structures for ever ten workers. There’s `dice: 1d6<=4` chance of having a blacksmith employed for every twenty workers, `dice: 1d6<=5` chance of having `dice: 2d4` mercenary guards for ever ten workers, and`dice: 1d6<=1` chance of having a 1st-level cleric present for every twenty workers. Camps with more than 100 workers have an equivalent Market Class of `dice: [[Fill#^LoggingMarket]]`                       |
| 36-38  | Military Garrison/Supply House. There’s `dice: 1d8<=1` chance that a garrison is treated as being a Market Class of `dice: [[Fill#^garrisonMarket]]` `dice: 1d6<=2` chance per twenty troops of having a cleric of level `dice: [[Fill#^GarrisonCleric]]` There’s `dice: 1d6<=1` chance per twenty-five troops of there being a magic-user of similar level. Additionally, there’s a `dice: 1d10<=1` chance that there will be 1 spy per twenty-five troops. These spies will be from  `dice: [[Fill#^garrisonSpy]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| 39-48  | Mill Will be `dice: [[Fill#^MillPower]]` Mills will process `dice: [[Fill#^MillMaterial]]`Water-powered lumber mills use blades driven by running water, while manually powered mills utilize teams of workers using pitsaws, or even splitting logs down into lumber. A typical lumber mill has `dice: 2d20` employees, plus draft horses to help move materials around. The workers will typically live adjacent to the mill, and there will be `dice: 1d2` support staff on hand for every five workers. This support staff includes laborers (`dice: 1d6>=5` chance per 5 workers), blacksmiths (`dice: 1d6>=3` chance per 5 workers), animal handlers (`dice: 1d6>=2` chance per 5 workers), etc.                                                                                                                                                                                                                                                                                           |
| 49-55  | Mine `dice: [[Fill#^MineType]]`A mine will be `dice: [[Fill#^MineOperator]]` Temporary settlements spring up around the mine, with workers living in tents or semi- permanent shelters. Mining camps attract support staff. Mines that are run by consortia or domains will have `dice: 1d6–1` guards for every ten miners. There will also be blacksmiths (1-3 in 6 chance per ten miners), animal handlers (`dice: 1d6>=2` chance per 25 miners), cooks (`dice: 1d6>=3` chance per ten miners), a rudimentary tavern (`dice: 1d6>=4` chance per fifty miners), etc. Mines will be visited every `dice: 1d4` weeks by supply caravans that bring supplies to the miners then return to settlements with ore. There’s `dice: 1d6>=2` chance per fifty workers that a mining camp has a smelter to process ore before shipping it away.                                                                                                                                                           |
| 56     | Monastery. Many monastic orders are headquartered in remote areas. They `dice: [[Fill#^MonasteryType]]` and will be `dice: [[Fill#^MonasteryAlignment]]`, Monasteries should be treated as the domains of name-level characters: strongholds founded by clerics (from the core rules) or assassins (p. 8, Advanced Fantasy). Use the rules in those books to determine the number of leveled characters present, and assume they have support staff equal to mining camps. Monasteries are also constructed as keeps and strongholds, usually `dice: [[Fill#^MonasteryMaterial]]`                                                                                                                                                                                                                                                                                                                                                                                                                |
| 57-65  | Orchard. Similar to farms, [[#Farm.]] but instead of planting seasonal crops the farmers tend orchards of `dice: [[Fill#^orchardType]]`, Because of the higher density and perennial nature of their crop subtract 10 from the roll when determining the size of the orchard. Orchards have  `dice: 1d6>=4` chance of being surrounded by a low wall, and `dice: 1d6>=2` chance of being patrolled by 1d4 guards for every ten acres. These guards are the equivalent of `dice: [[Fill#^OrcharGuards]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 66-70  | Other. Get creative                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 71-75  | Quarry `dice: [[Fill#^QuarryType]]`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 76-85  | Ranch In all other respects similar to farms, [[#Farm.]] but ranches primarily raise livestock. Ranches have `dice: 1d6>=2` chance of being surrounded by wooden fences with a primary purpose of keeping animals in rather than protecting the property from external threats. Add 10 to the roll when determining the ranch size. If the result is 101 or above the ranch is 1d4 subhexes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 86-95  | Shrine. Unlike temples, that are staffed by priests of a deity, shrines are smaller structures dedicated to a deity. There are typically no full-time attendants of a shrine, although there may be a part-time caretaker that occasionally visits the shrine to look after the place. The shrine will be dedicated to a `dice: [[Fill#^MonasteryAlignment]]` Diety. There’s `dice: 1d6>=3` chance there’s a semi-permanent caretaker that visits every  `dice: [[Fill#^ShrineAttendant]]`. It will be `dice: [[Fill#^ShrineSize]]` There’s `dice: 1d6>=3` chance the shrine possesses divine properties that will take effect `dice: [[Fill#^ShrineTrigger]]`, These effects usually take the form of a bane or a boon; banes occur when, for instance, a Chaotic creature enters the grounds of a Lawful shrine. Banes will impose the following: `dice: [[Fill#^ShrineBane]]`. Banes last for `dice: [[Fill#^ShrineBaneDuration]]` `dice: [[Fill#^BaneDispel]]`, `dice: [[Fill#^ShrineBoon]]` |
| 96-100 | Temple. Temples are larger than shrines, with a permanent contingent of worshipers. Temples have the same proportions of alignments as shrines. Like monasteries, temples should be treated as name-level strongholds run by clerics or paladins. Use the rules in the OSE rulebooks to determine the number of followers. There will be support staff in the temple equal to `dice: 3d4*10`% of the followers. The support staff may be generally followers of the deity, but are considered to be 0-level NPCs. `dice: [[Fill#^TempleArchitecture]]`. Every temple contains a shrine that has `dice: 1d6>=2` chance of having divine properties similar to other shrines, above.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
^CommercialType

There’s a 1 in 6 chance in Wilderness hexes that the infrastructure is (1-4) abandoned and potentially used as a lair for monsters or (5-6) under attack or threat.
| dice: 1d36 |                                                      |
| ---------- | ---------------------------------------------------- |
| 1-30       | Infrastructure is used as purpose                    |
| 31-34      | abandoned and potentially used as a lair for monster |
| 35-36      | under attack or threat.                                                     |
^CommercialAbandoned

Features in this category will be inhabited by 

| dice: 1d8 |                                                                                                           |     |
| --------- | --------------------------------------------------------------------------------------------------------- | --- |
| 1-4       | Men,                                                                                                      |     |
| 5-6       | demi-humans,                                                                                              |     |
| 7         | humanoids,                                                                                                |     |
| 8         | other races, who may *appear* differently than they truly are (doppelgangers, polymorphed dragons, etc.). |     |
^commercialinhabitants

The commercial infrastructure’s age will be . . .



33-table-1.md

| d100   | Result        |
|:-------|:--------------|
| 1-10   | 1d10 years    |
| 11-60  | 10d10 years   |
| 61-99  | 10d100 years  |
| 100    | 10d1000 years |

[[Fill#^monumentAge]]

###### Camps. 
Camps are either 

| dice: 1d12 |                        |
| ---------- | ---------------------- |
| 1-5        | occupied by  travelers |
| 6          | occupied by squatters  |
| 7-12       | currently empty.       |
^CampOccupied


Camps are maintained by either the local domain ruler, merchant guild, or military to provide designated areas for military or mercantile caravans to rest while traveling. They usually are found on flat, raised ground, marked in some fashion. 
Camps have a
`dice: 1d6<5` chance of having low defensive walls surrounding the perimeter (`dice: 1d4+2` feet tall). 
There is also `dice: 1d6<3` chance someone has been nice enough to keep a stock of dry firewood. 
`dice: 1d6<2` camps have semi-permanent, crude shelters for animals or Man, and 

1-4 in 6 of them will have a nearby source of water in the form of a

| dice: 1d18 |                        |
| ---------- | ---------------------- |
| 1-4        | stream,                |
| 5-8        | spring,                |
| 9-10       | fountain, or           |
| 11-12      | well.                  |
| 13-18      | nearby source of water |
^campwatersource

###### Farm. 
A farm will be the following size . . .

33-table-2.md

| d100   | Result              |
|:-------|:--------------------|
| 1-10   | Smaller than 1 acre |
| 11-20  | `dice: 1d4` acres           |
| 21-50  | `dice: 2d6` acres           |
| 51-75  | `dice: 3d8` acres           |
| 76-90  | `dice: 4d10` acres          |
| 91-95  | `dice: 5d12` acres `dice: 1d6<5` chance of being a market with a Class of 1.          |
| 96-100 | `dice: 6d20` acres `dice: 1d6<5` chance of being a market with a Class of 1. Farms that are over 100 acres will be a market of Class `dice: [[Fill#^Farmmarketclass]]`.        |
^FarmSize


If the farm is found in a forested, swamp, jungle, or mountain hex subtract 10 from the roll.

All farms, in addition to growing crops, will keep a variety of animals. Chickens for eggs, pigs to forage and eat scraps, horses, mules, or oxen to work the fields, etc. The primary focus of the farmer is on growing crops, though. Most farms grow a variety of plants, instead of one single crop, and they will typically be working from early spring through late fall planting, harvesting, and preparing food for storage. 

Surplus crops are 

| dice: 1d6 |                                                        |
| --------- | ------------------------------------------------------ |
| 1-4       | taken to the nearest market to sell or                 |
| 5-6       | tithed to the domain ruler (if in an existing domain). |
^Surplus

The smallest farms consist of a single family living in one or two buildings. The larger a farm gets the more hands are needed to run it, and the more infrastructure is needed to support the operation. Large farms will typically consist of 1d2 buildings for every ten acres under cultivation. These buildings include: houses for the farmers (typically a main house for the owners, plus smaller outbuildings that the workers live in), smithies/workshops to repair equipment, barns to house livestock, smokehouses to cure meat, root cellars to preserve harvested food, granaries or silos to store grain, etc.

Large farms, especially those encountered in Wilderness hexes, function as small settlements, are often protected by walls, and often serve as waystations or inns for travelers to rest in, whether they sleep in a barn or there is a dedicated building for use by travelers.

Farms that are larger than 50 acres may be large enough to have supplies available for sale. Such farms have a 


Farms that are over 100 acres will be a market of Class `dice: [[Fill#^Farmmarketclass]]`.

| dice: 1d6 |                    |
| --------- | ------------------ |
| 1-4       | market of Class 1  |
| 5-6       | market of Class 2. |
^Farmmarketclass

Refer to the section on Resources for more information on crop type.

###### Ferry. 
Reroll if this result comes up when it is not appropriate. Ferries are used to cross rivers when bridges are not available. 

The ferry will be

| dice: 1d6 |                                                                                                                                         |
| --------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| 1-3       | operated by the user, `dice: [[Fill#^ferryselfservice]]`                                                                                |
| 4-5       | operated by a dedicated ferryman, or                                                                                                    |
| 6         | operated by some other means. Ferries operated by other means could be poled by constructs, powered by spells, or other exotic devices. |
^ferryoperator

Those operated by the user usually consist of a raft or flat-bottomed boat that runs on a rope strung across the river. The boat is pulled or poled across and can be pulled back by travelers as needed. These self-service ferries have a 



| dice: 1d18 |                                                                 |
| ---------- | --------------------------------------------------------------- |
| 1-12       |                                                                 |
| 13-16      | being out of service due to neglect or vandalism, or            |
| 17-18      | operated by bandits or brigands looking to prey upon travelers. |
^ferryselfservice

Increase this chance by 1 in Wilderness hexes.

If the ferry is operated by a ferryman they, and potentially their family, live nearby, and they live off the income generated by transporting travelers. Fees for transport will be . . .



33-table-3.md

| d100   | Result                     |
|:-------|:---------------------------|
| 1-25   | 1d8 cp                     |
| 26-75  | 1d8 sp                     |
| 76-99  | 1d8 gp                     |
| 100    | Something other than money |
^ferryfee

In Wilderness hexes add 10 to the roll. 

Ferry boats will be capable of transporting 


| dice: 1d6 |                                                                  |
| --------- | ---------------------------------------------------------------- |
| 1-3       | `dice: 2d4` individuals at a time, or half that number of mounts |
| 4-5       | `dice: 3d6` individuals at a time, or half that number of mounts |
| 6         | `dice: 3d8` individuals at a time, or half that number of mounts |
capacity


individuals at a time, or half that number of mounts, so it may take multiple trips. 

Ferrymen have a 
1 in 20 chance of proving unscrupulous, either 



| dice: 1d120 |                                                                        |     |     |
| ----------- | ---------------------------------------------------------------------- | --- | --- |
| 1-114       | ferryman honest                                                        |     |     |
| 115-117     | ferryman working with brigands,                                        |     |     |
| 118-119     | ferryman stranding half the party on either side and insisting on more payment, |     |     |
| 120         | ferryman is some sort of monster in disguise.                                |     |     |
^dishonestferryman

Ferries operated by other means could be poled by constructs, powered by spells, or other exotic devices.

Depending on the weather or season a ferry may not be operable. Heavy rains or melting snow cover may render the river too dangerous to cross, and obviously a frozen river does not need a ferry, provided the ice is thick enough to walk across.

###### Ford. 
Simply a shallow part of a river or large stream, fords allow for travelers to cross in relative safety, albeit while getting wet. 

There’s `dice: 1d6<3` chance that the crossing is dangerous during certain times of the year, or after heavy rain. In these cases those crossing must succeed on a Save v. Death to avoid being swept off their feet. If the travelers are mounted while crossing their mounts make the save, but with a +2 bonus to the roll.

If a ford is frequently used there’s `dice: 1d20<2` chance it is watched by brigands or monsters who use the distraction of crossing to attack. This chance is reduced to 1 in 100 in Civilized hexes.

Fords are 

| dice: 1d6 |                                                 |
| --------- | ----------------------------------------------- |
| 1-4       | naturally occurring shallow spots in a river or |
| 5-6       | man-made.                                       |
^fordmanmade

Because they are shallower they are also wider, which may be important to know if travelers are trying to cross swiftly. Assume that a ford is roughly twice as wide as other parts of the river.

A ford will be . . .



34-table-1.md

| d100   | Result                                                                                             |
|:------ |:-------------------------------------------------------------------------------------------------- |
| 1-50   | `dice: 1d4` feet deep                                                                                      |
| 51-90  | `dice: 2d4` feet deep Fords that are deeper than five feet are typically only crossed by mounted travelers |
| 91-100 | `dice: 3d4` feet deep Fords that are deeper than five feet are typically only crossed by mounted travelers |
^forddepth

Fords that are deeper than five feet are typically only crossed by mounted travelers, and are used simply because the wider, shallower part of the river is slower moving than other areas.

###### Hunting Lodge. 
Hunting lodges are maintained for three distinct reasons: 

| dice: 1d6 |                                                                                               |
| --------- | --------------------------------------------------------------------------------------------- |
| 1-3       | maintained by trappers and hunters to use as a base of operations,                                       |
| 4-5       | maintained by nobles that maintain the house for use during sport hunting, or                            |
| 6         | maintained by name-level ranger-type characters that use it as a base of operations in Wilderness hexes. |
^LodgeOwner

Hunting lodges consist of `dice: 1d4` buildings, typically of `dice: [[Fill#^LodgeMaterial]]`

| dice: 1d6 |                 |
| --------- | --------------- |
| 1-3       | wood,           |
| 4-5       | stone, or       |
| 6         | other material. |
^LodgeMaterial

Because they are often forced to rely on their own supplies for long periods of time there’s `dice: 1d6<3` chance that a hunting lodge has a Market Class of 1.

###### Inn
Found mostly along heavily trafficked trade routes where there is not enough population to support a community, but enough travel to support a business, roadside inns in Borderland or Wilderness hexes are most often fortified complexes with walls that enclose the main inn and outbuildings. Roadside inns have 1d8 features in Borderland hexes and 2d6 in Wilderness hexes (roll 1d00 to determine the features), listed below. Unless otherwise indicated results are cumulative.

`dice: 1d8[[Fill#^innFeature]]`

34-table-2.md

| d100   | Result                                                                                                                                                                                                                                                                                                                                                                        |
|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1-31   | Guards. `dice: 1d6+1` guards are in the employ of the  inn.  Treat  as `dice [[Fill#^InnGuards]]`. Every 4 guards will be overseen by a sergeant one level higher. Ex. Five  crossbowmen  will  be  overseen  by  a  1st-level fighter, while four 1st-level fighters will be overseen by a 2nd-level fighter. |
| 32-33  | Guild  Hideout.  The  inn  is  in  fact  a  cover for the local thieves’  guild.  Most  of the employees will knowingly work for or be in the employ of the guild. Refer to the Guide to Thieves’ Guilds for more information.                                                                                                                                                |
| 34-36  | Hirelings. Potential employees can be found at  the  inn.  There  will  be  either `dice: [[Fill#^InnHirelings]]`  available  for  hire  at  any  given  time.  If  this result comes up more than once increase the number of potential hirelings by 1.                                                                                             |
| 37-38  | Magic-user.  The  inn  has  a  magic-user  on staff.  While  primarily employed  by the innkeeper  the  magic-user  can  be  hired  to cast  spells  for  the  PCs. The  magic-user  will be `dice: [[Fill#^InnCaster]]`If  this  result  comes  up  twice  increase the NPC’s level by 1.                                                          |
| 39     | Magical  item.  There  is  one  magical  item available for sale or trade (in exchange for a service). This will be `dice: [[Fill#^InnItem]]`                                                                                                                                                                                                      |
| 40-49  | Market. The inn serves as the urban center for nearby residents and has a Market Class of 1. Each time this result comes up add 1 to the Market Class.                                                                                                                                                                                                                        |
| 50-57  | Smithy.  The  smithy  will  be  run  by  a `dice: [[Fill#^InnSmith]]` .  If  this  result comes  up  more than  once assume the additional workers are assistants.                                                                                                                                                                                                   |
| 58-59  | Spy. One of the workers at the inn is a spy, sponsored by `dice: [[Fill#^InnSpy]]`                                                                                                                            |
| 60-72  | Stables. The inn maintains enclosed stables and stablehands that care for the mounts of travelers. There’s `dice: 1d6<4` chance there will be  `dice: 1d4`  randomly  determined  mounts  for sale, and `dice: [[Fill#^InnWagon]]` for sale.                                     |
| 73-77  | Temple.  The  inn  maintains  a  small  temple that is overseen by a `dice: [[Fill#^InnTemple]]` If this  result  occurs  more  than  once  increase the level of the cleric by 1.                                                                 |
| 78-79  | Threat.  A  hidden  threat  lurks  in  the  inn. One  or  more  of  the  staff  may  be  disguised monsters, or the food may have spoiled and will poison the guests, or a fire may break out at  night.  If  this  result  comes  up  more  than once increase the threat level appropriately. |
| 80-100 | Wall.  The inn is  surrounded  by  a `dice: [[Fill#^InnWall]]` wall  that is  approximately  eight feet tall.  For  each additional result add another defensive feature (arrow slits, moat, tower, etc.).                                                                    |
^innFeature


| dice: 1d6 |                    |
| --------- | ------------------ |
| 1-3       | footmen,  light,   |
| 4-5       | footmen,  heavy,   |
| 6-7       | crossbowmen,  or   |
| 8         | 1st-level fighters |
^InnGuards


| dice: 1d6 |                                 |
| --------- | ------------------------------- |
| 1-4       | `dice: 1d4` mercenaries or      |
| 5-6       | `dice: 1d2` potential retainers |
^InnHirelings

| dice: 1d6 |            |
| --------- | ---------- |
| 1-3       | 1st level, |
| 4-5       | 2nd level, |
| 6         | 3rd level. |
^InnCaster



| dice: 1d6 |                        |
| --------- | ---------------------- |
| 1-4       | a potion or scroll, or |
| 5-6       | a permanent item       |
^InnItem

| dice: 1d6 |            |
| --------- | ---------- |
| 1-5       | blacksmith |
| 6         | armorer    |
^InnSmith

| dice: 1d6 |                            |
| --------- | -------------------------- |
| 1-2       | the nearby domain ruler,   |
| 3-4       | a  foreign  domain  ruler, |
| 5         | a  band  of brigands, or   |
| 6         | other.                     |
^InnSpy


| dice: 1d18 |              |
| ---------- | ------------ |
| 1-12       | nothing more |
| 16-17      | cart         |
| 18         | wagon        |
^InnWagon

| dice: 1d6 |                      |
| --------- | -------------------- |
| 1-3       | 1st-level cleric,    |
| 4-5       | 2nd-level cleric,|
| 6         | 3rd-level cleric.    |
^InnTemple


| dice: 1d6 |            |
| --------- | ---------- |
| 1-3       | wood,      |
| 4-5       | brick,  or |
| 6         | stone      |
^InnWall


###### Lighthouse/signal towers.
Tall buildings with a light atop to 

| dice: 1d6 |                                                                                                                                                                                                      |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-4       | guide travelers Lighthouses are kept continually lit at night or cloudy days to warn nearby ships of dangers in the vicinity.                                                                     |
| 5-6       | send messages. Signal towers are typically maintained by `dice: [[Fill#^TowerMaintainer]]`, They will be spaced out at increments of three miles plus 1.5 for every ten feet in height of the tower. |
^Signatower

The towers will be `dice: 3d6*10` feet high and manned by `dice: 1d4` staff with a `dice: 1d6<=4` chance of having `dice: 2d4` mercenary guards. 

Signal towers are typically maintained by 

| dice: 1d6 |                      |
| --------- | -------------------- |
| 1-5       | domain rulers or     |
| 6         | other organizations. |
^TowerMaintainer

They will be spaced out at increments of three miles plus 1.5 for every ten feet in height of the tower. The fire is 

| dice: 1d6 |                                |
| --------- | ------------------------------ |
| 1-4       | only lit in times of danger or |
| 5-6       | lit to send coded messages.    |
^WhenOn


Lighthouses are kept continually lit at night or cloudy days to warn nearby ships of dangers in the vicinity.

###### Logging Camp.
When found in wooded areas such a camp is dedicated to cutting timber; when found in non-wooded areas the workers harvest sod, peat, or similar material. An ocean-side camp may harvest kelp or something similar. The camp will 


| dice: 1d6 |                                    |
| --------- | ---------------------------------- |
| 1-3       | ship harvested material via river, |
| 4- 5      | sell it for use nearby, or         |
| 6         | ship it via land.                  |
^LoggingConnections

Refer to the Resource section on p. 37 to determine the value/size of nearby resources. There will be `dice: 1d6` individuals dedicated to harvesting the material for every subhex of resource. Camps will be 

| dice: 1d6 |                             |
| --------- | --------------------------- |
| 1-5       | semi-permanent dwellings or |
| 6         | permanent structures.       |
^LoggingPermanent

There will be `dice: 1d2` structures for ever ten workers. There’s `dice: 1d6<=4` chance of having a blacksmith employed for every twenty workers, `dice: 1d6<=5` chance of having `dice: 2d4` mercenary guards for ever ten workers, and`dice: 1d6<=1` chance of having a 1st-level cleric present for every twenty workers. Camps with more than 100 workers have an equivalent Market Class of 


| dice: 1d6 |      |
| --------- | ---- |
| 1-4       | 1 or |
| 5-6       | 2.   |
^LoggingMarket

There’s `dice: 1d6<=2` chance that a logging camp has a lumber mill (see below) as part of the camp. This chance is increased by 1 in Wilderness hexes.

###### Military Garrison/Supply House. 
Large domains often maintain barracks or garrisons on their borders to project their power into Borderlands or Wilderness areas outside of the domain proper. These are to be treated as keeps, housing a military garrison of the appropriate size based upon the size of the keep. [[#Tower/Keep/Castle]]

Garrisons will also contain a surplus of supplies for the forces to use should they be under attack or need to march to war. Each garrison will have a supply of dried rations, weapons, and ammunition that can be drawn from to supply troops.

There’s `dice: 1d8<=1` chance that a garrison is treated as being a Market Class of

| dice: 1d6 |                    |
| --------- | ------------------ |
| 1-4       | Market Class of 1  |
| 5-6       | Market Class of 2. |
^garrisonMarket

There’s an additional 


`dice: 1d6<=2` chance per twenty troops of having a cleric of level 

| dice: 1d6 |       |
| --------- | ----- |
| 1- 3      | 1,    |
| 4-5       | 2, or |
| 6         | 3.    |
^GarrisonCleric

There’s `dice: 1d6<=1` chance per twenty-five troops of there being a magic-user of similar level. Additionally, there’s a `dice: 1d10<=1` chance that there will be 1 spy per twenty-five troops. These spies will be from 

| dice: 1d6 |                                                        |
| --------- | ------------------------------------------------------ |
| 1-3       | the domain ruler, keeping an eye on corruption,        |
| 4         | an outside domain,                                     |
| 5         | a local thieves’/brigands’ guild, or                   |
| 6         | an evil cult, enemy, or polymorphed/disguised monster. |
^garrisonSpy


###### Mill. 
Mills will be 

| dice: 1d6 |                                            |                       |      |
| --------- | ------------------------------------------ | --------------------- | ---- |
| 1-3       | powered by moving water,                   |                       |      |
| 4-5       | powered by manual labor                    | animals, slaves, etc. | , or |
| 6         | powered by another source, likely magical. |                       |      |
^MillPower

Mills will process 

| dice: 1d6 |                                                                                                                                                                                                                                                                                                                           |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-3       | grain, Grain mills will only be found in Wilderness hexes on a roll of 1-2 in 6 as they overwhelmingly tend to be in more densely populated areas where they can serve the needs of a larger community of farmers. Grain mills tend to be small operations, attached to dwellings where the miller and their family live. |
| 4-5       | timber, or Lumber mills, on the other hand, are often found in Borderlands or Wilderness hexes as it is easier to mill nearby timber and then ship it for use in new construction, rather than import the raw material. These are larger operations, requiring intensive labor to process felled trees.                   |
| 6         | other material.                                                                                                                                                                                                                                                                                                           |
^MillMaterial


Water-powered lumber mills use blades driven by running water, while manually powered mills utilize teams of workers using pitsaws, or even splitting logs down into lumber. A typical lumber mill has `dice: 2d20` employees, plus draft horses to help move materials around. The workers will typically live adjacent to the mill, and there will be `dice: 1d2` support staff on hand for every five workers. This support staff includes laborers (`dice: 1d6>=5` chance per 5 workers), blacksmiths (`dice: 1d6>=3` chance per 5 workers), animal handlers (`dice: 1d6>=2` chance per 5 workers), etc.

###### Mine. 
Mines are 



| dice: 1d6 |                                                                                                                                                                                                                                                                                                                                                       |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-3       | dug mines. Dug mines are created by digging shafts into the ground that follow veins of minerals. They can descend deep into the earth, and require physical bracing and reinforcement. The deeper a dug mine goes the more labor is needed to efficiently extract materials, and the more dangerous it becomes. dug mines have `dice: 1d100` workers |
| 4-5       | sluice. Sluice mines rely on exposing surface minerals with running water, either by blasting surface dirt with pressurized water or by panning to separate heavier minerals. Sluice mines have `dice: 1d8` workers                                                                                                                                   |
| 6         | strip mines. Strip mines also require digging, but instead of digging narrow tunnels that follow the path of mineral veins they rely on removing large amounts of earth to exposed seams of valuable minerals. strip mines `dice: 5d100`workers                                                                                                       |
^MineType

A mine will be 

| dice:1d6 |                                                         |
| -------- | ------------------------------------------------------- |
| 1-3      | a solo operation, run by a single individual or family, |
| 4-5      | a larger operation owned as a mercantile venture, or    |
| 6        | owned by a nearby ruler, noble, or landowner.           |
^MineOperator






Sluice mines have `dice: 1d8` workers, dug mines have `dice: 1d100` workers, and strip mines `dice: 5d100`workers. Temporary settlements spring up around the mine, with workers living in tents or semi- permanent shelters. Mining camps attract support staff. Mines that are run by consortia or domains will have `dice: 1d6–1` guards for every ten miners. There will also be blacksmiths (1-3 in 6 chance per ten miners), animal handlers (`dice: 1d6>=2` chance per 25 miners), cooks (`dice: 1d6>=3` chance per ten miners), a rudimentary tavern (`dice: 1d6>=4` chance per fifty miners), etc.

Mines will be visited every `dice: 1d4` weeks by supply caravans that bring supplies to the miners then return to settlements with ore. There’s `dice: 1d6>=2` chance per fifty workers that a mining camp has a smelter to process ore before shipping it away.

Refer to the section on Resources on p. 37 for more information.

###### Monastery. 
Many monastic orders are headquartered in remote areas. They 

| dice: 1d6 |                                                      |     |
| --------- | ---------------------------------------------------- | --- |
| 1-3       | are primarily religious,                             |     |
| 4-5       | are primarily martial, or                                |     |
| 6         | are primarily esoteric (specializing in magical research | .   |
^MonasteryType

They will be 

| dice:1d6 |             |
| -------- | ----------- |
| 1-2      | Lawful,     |
| 3-4      | Neutral, or |
| 5-6      | Chaotic.    |
^MonasteryAlignment

Monasteries should be treated as the domains of name-level characters: strongholds founded by clerics (from the core rules) or assassins (p. 8, Advanced Fantasy). Use the rules in those books to determine the number of leveled characters present, and assume they have support staff equal to mining camps. Monasteries are also constructed as keeps and strongholds, usually 


| dice:1d6 |                                     |
| -------- | ----------------------------------- |
| 1-4      | of stone or brick, but occasionally |
| 5-6      | of wood or other materials.         |
^MonasteryMaterial

Otherwise, monasteries are built along the lines of dungeons.

###### Orchard.
Similar to farms, [[#Farm.]] but instead of planting seasonal crops the farmers tend orchards of 

| dice:1d6 |               |
| -------- | ------------- |
| 1-3      | fruit trees,  |
| 4-5      | nut trees, or |
| 6        | grape vines.  |
^orchardType

Because of the higher density and perennial nature of their crop subtract 10 from the roll when determining the size of the orchard. Orchards have  `dice: 1d6>=4` chance of being surrounded by a low wall, and `dice: 1d6>=2` chance of being patrolled by 1d4 guards for every ten acres. These guards are the equivalent of 


| dice:1d6 |               |
| -------- | ------------- |
| 1-4      | light foot or |
| 5-6      | heavy foot.   |
^OrcharGuards

###### Other.
Use this category for features that are not included in any of the others.

###### Quarry.
Quarries are similar to mines, except they are usually 

| dice: 1d6 |                                                 |
| --------- | ----------------------------------------------- |
| 1-5       | of the strip mine variety, and only very rarely |
| 6         | dug mines.                                      |
^QuarryType

Refer to the section on Resources, below.

###### Ranch.
In all other respects similar to farms, [[#Farm.]] but ranches primarily raise livestock. Ranches have `dice: 1d6>=2` chance of being surrounded by wooden fences with a primary purpose of keeping animals in rather than protecting the property from external threats. Add 10 to the roll when determining the ranch size. If the result is 101 or above the ranch is 1d4 subhexes.


###### Shrine. 
Unlike temples, that are staffed by priests of a deity, shrines are smaller structures dedicated to a deity. There are typically no full-time attendants of a shrine, although there may be a part-time caretaker that occasionally visits the shrine to look after the place. The shrine will be dedicated to a [[Fill#^MonasteryAlignment]] Diety.


There’s `dice: 1d6>=3` chance there’s a semi-permanent caretaker that visits every 


| dice:1d6 |                      |
| -------- | -------------------- |
| 1- 3     | `dice: 1d4` weeks,   |
| 4-5      | `dice: 1d8` days, or |
| 6        | `dice: 1d4` months.  |
^ShrineAttendant

The shrine will be 


| dice:1d6 |                                       |
| -------- | ------------------------------------- |
| 1-3      | a statue, object, or natural feature, |
| 4-5      | a single room or rudimentary shelter, |
| 6        | a building with `dice: 1d4+1` rooms.  |
^ShrineSize


There’s `dice: 1d6>=3` chance the shrine possesses divine properties that will take effect 


| dice:1d6 |                                                     |
| -------- | --------------------------------------------------- |
| 1        | whenever someone of a certain alignment enters,     |
| 2        | whenever something is left or taken,                |
| 3        | upon everyone who enters,                           |
| 4        | if a specific action is taken within the shrine, or |
| 5-6      | other.                                              |
^ShrineTrigger


These effects usually take the form of a bane or a boon; banes occur when, for instance, a Chaotic creature enters the grounds of a Lawful shrine. Banes will impose the following: 


| dice:1d6 |                                                                                            |                                 |     |
| -------- | ------------------------------------------------------------------------------------------ | ------------------------------- | --- |
| 1        | the offending creature suffers a penalty of `dice: 1d4` to a specific roll,                |                                 |     |
| 2        | the offending creature automatically rolls the lowest possible result on their next roll,  |                                 |     |
| 3        | the offending creature must Save v. Spells or have their alignment change to its opposite, |                                 |     |
| 4        | the offending creature must Save v. Polymorph or be turned into another form               | stone, or ooze, or animal, etc. | ,   |
| 5        | the offending creature is targeted by the geas spell, or                                   |                                 |     |
| 6        | other.                                                                                     |                                 |     |
^ShrineBane

Banes last for 


| dice:1d6 |                       |
| -------- | --------------------- |
| 1- 3     | `dice: 1d8` days,     |
| 4-5      | `dice: 1d4` weeks, or |
| 6        | permanently.          |
^ShrineBaneDuration

They can be removed by 

| dice:1d6 |                                                                     |
| -------- | ------------------------------------------------------------------- |
| 1        | a remove curse cast by a cleric of level `dice: 1d6+8` or higher,   |
| 2        | a dispel magic cast by a spellcaster of at least level`dice: 1d6+8` |
| 3        | a wish or similar magic,                                            |
| 4        | divine intervention,                                                |
| 5        | undoing whatever action triggered the bane, or                      |
| 6        | other.                                                              |
^BaneDispel



Boons impose the following: 

| dice:1d6 |                                                                          |
| -------- | ------------------------------------------------------------------------ |
| 1        | the subject gains a bonus of `dice: 1d4` to a specific roll,             |
| 2        | the subject automatically succeeds on their next roll,                   |
| 3        | the subject gains a bonus `dice: 1d6` hit points,                        |
| 4        | the subject has one random ability score improved by 1,                  |
| 5        | the subject gains a bonus ability congruent with the god’s portfolio, or |
| 6        | other.                                                                   |
^ShrineBoon

Note that boons and banes that specifically call out “the next roll” do not permanently grant the modifier, but will expire once that next roll is made, regardless of how long it takes to make that roll.


###### Temple.
Temples are larger than shrines, with a permanent contingent of worshipers. Temples have the same proportions of alignments as shrines. Like monasteries, temples should be treated as name-level strongholds run by clerics or paladins. Use the rules in the OSE rulebooks to determine the number of followers. There will be support staff in the temple equal to `dice: 3d4*10`% of the followers. The support staff may be generally followers of the deity, but are considered to be 0-level NPCs.

Temples can be 


| dice:1d6 |                                                            |
| -------- | ---------------------------------------------------------- |
| 1-3      | a single large structure divided in `dice: 3d6` rooms,     |
| 4-5      | an enclosed campus containing `dice: 2d6` outbuildings, or |
| 6        | a military-style keep.                                     |
^TempleArchitecture


Every temple contains a shrine that has `dice: 1d6>=2` chance of having divine properties similar to other shrines, above.


#### Barriers
Barriers are structures and features, both natural and man-made, that somehow block or impede progress. Barriers are either 

| dice: 1d6 |                                                                         |
| --------- | ----------------------------------------------------------------------- |
| 1-3       | natural. Natural barriers include `dice: [[Fill#^NaturalBarriers]]`     |
| 4-5       | man-made barriers include `dice: [[Fill#^ManMadeBarriers]]`             |
| 6         | magical. Magical barriers include `dice: [[Fill#^MagicalBarriersType]]` |
^barriertype

The purpose of this section is to provide obstacles that slow the adventurers’ progress.

When a barrier is rolled determine what the nature of the barrier is (man-made, natural, etc.), pick a barrier that works best with the hex, and refer to the appropriate section in this book. Barriers, if the adventurers insist on continuing on their path, will slow progress by . . .


37-table-1.md

| dice: 1d100 | Result                                                                                                                                                                                       |
|:----------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-50        | 25%                                                                                                                                                                                          |
| 51-75       | 50%                                                                                                                                                                                          |
| 76-95       | 75%                                                                                                                                                                                          |
| 96-100      | 100% Barriers that slow progress by 100% create zones (see below) that cannot be explored until the barrier is overcome. Otherwise, assume the zone can be explored, but at the slower rate. |
^BarrierIntensity

Barriers that slow progress by 100% create zones (see below) that cannot be explored until the barrier is overcome. Otherwise, assume the zone can be explored, but at the slower rate. Each barrier affects a “zone”, or a certain area. The smallest area a zone can affect is a single subhex. Roll below to determine the size of the zone . . .


38-table-2.md

| dice: 1d100 | Result               |
|:----------- |:-------------------- |
| 1-40        | 1 subhex             |
| 41-70       | `dice: 1d4` subhexes |
| 71-85       | `dice: 3d4` subhexes |
| 86-95       | `dice: 4d6` subhexes |
| 96-100      | `dice: 1d4` hexes    |
^BarrierZone

38-table-4.md

Natural barriers include . . .

| dice: 1d100 | Result               |
|:----------- |:-------------------- |
| 1-15        | Boggy/marshy terrain |
| 16-30       | Canyons              |
| 31-45       | Cliffs               |
| 46-60       | Impenetrable foliage |
| 61-75       | Rivers               |
| 76-100      | Other                |
^NaturalBarriers


Natural barriers can be treated either as a terrain type that slows movement (and potentially renders certain types of transportation, such as wagons or boats, unusable) or as a hazard (see p. 45)

Man-made barriers include . . .


38-table-5.md

| dice: 1d100 | Result                   |
|:----------- |:------------------------ |
| 1-40        | Traps. Refer to p.       |
| 41-60       | Trenches. Refer to p. 22 |
| 61-80       | Walls. Refer to p. 21    |
| 81-100      | Other.                   |
^ManMadeBarriers

Man-made barriers can be overcome in the normal fashion.


Magical barriers include . . .

38-table-1.md

| dice: 1d100 | Result                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|:----------- |:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-20        | Force fields. A force field is an `dice: [[Fill#^forcefieldVisible]]` thin magical barrier that is the result of a `dice: [[Fill#^ForcefieldOrigin]]` It cannot be breached by physical means, and there’s `dice: 1d6 <=4` chance it is impervious to magical effects, including those that do not create physical results (such as charm person).  There’s a further `dice: 1d6 <=1` chance that touching the force field inflicts injury upon the one touching it, as follows `dice: [[Fill#^ForcefieldDMGAmount]]`, `dice: [[Fill#^ForcefieldDMGType]]` damage. When rolling to determine the size of a force field [[#^BarrierZone]] , subtract 20 from the roll. On a result of less than 1, the force field occupies `dice: 1d10*1000` sq. ft. Force fields will `dice: [[Fill#^ForcefieldBypass]]`. If targeted by a spell such as dispel magic treat the force field as being of a spell level equal to `dice: 1d6+4`. There’s an additional `dice: 1d6<=1` chance that a force field completely surrounds (above and below ground) an area; otherwise it simply rises to a height of `dice: 1d100` feet. |
| 21-40       | Illusory images/terrain. Illusory images or terrain should be treated as spells such as hallucinatory terrain, massmorph, or other illusion spells. Allow those passing through the illusion to roll `dice: 4d6` and compare the result to their Intelligence score. If the result is equal to or less than their score they are able to determine that there is an illusion. Illusions are the result of `dice: [[Fill#^IllusionOrigin]]`. Treat the illusion as if it were a spell of level `dice: 1d8+1`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 41-60       | Magical walls (of fire, stone, etc.). Magical walls are just that: barriers created by such spells as wall of stone, wall of fire, etc., or potentially other spells such as acid fog, cloudkill, etc.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| 61-80       | Zones of repulsion. Zones of repulsion are invisible barriers that are otherwise treated as force fields, except they can be crossed. Once inside, an affected individual must make a saving throw against spells for every turn spent inside or be compelled to leave by the fastest means possible. Zones of repulsion have only a `dice: 1d6 <=1` chance of affecting *all* creatures that enter. Otherwise, roll below to determine what manner of creatures are affected: `dice: [[Fill#^RepulsionTarget]]`. There’s a further `dice: 1d6<=1` chance that a specific creature type is affected by the barrier (goblins, rather than all humanoids).                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 81-100      | Other                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
^MagicalBarriersType

1-20. A force field is an 

| dice: 1d6 |           |
| --------- | --------- |
| 1-2       | invisible |
| 3-6       | visible,  |
^forcefieldVisible



| dice: 1d6 |                      |
| --------- | -------------------- |
| 1-2       | spell,               |
| 3-5       | magical artifact, or |
| 6         | other phenomenon.    |
^ForcefieldOrigin

It cannot be breached by physical means, and there’s `dice: 1d6 <=4` chance it is impervious to magical effects, including those that do not create physical results (such as charm person).  There’s a further `dice: 1d6 <=1` chance that touching the force field inflicts injury upon the one touching it, as follows: 

38-table-3.md

| dice: 1d8 | Result                                 |
|:--------- |:-------------------------------------- |
| 1-3       | `dice: 1d6` points of damage (no save) |
| 4-5       | `dice: 2d6` points of damage (no save) |
| 6-7       | `dice: 3d6` points of damage (no save) |
| 8         | Save vs. spells or be disintegrated.   |
^ForcefieldDMGAmount


Damage will be 

| dice: 1d6 |                            |
| --------- | -------------------------- |
| 1-3       | electrical,                |
| 4-5       | force, or                  |
| 6         | some other type of energy. |
^ForcefieldDMGType

When rolling to determine the size of a force field [[#^BarrierZone]] , subtract 20 from the roll. On a result of less than 1, the force field occupies `dice: 1d10*1000` sq. ft. Force fields will 

| dice: 1d6 |                                                                                                 |
| --------- | ----------------------------------------------------------------------------------------------- |
| 1-3       | have a means of temporarily disabling them accessible to the adventurers,                       |
| 4-5       | have a means of bypassing them such as via specifically made magical items or unique spells, or |
| 6         | have no means of bypassing short of brute magical force.                                        |
^ForcefieldBypass

If targeted by a spell such as dispel magic treat the force field as being of a spell level equal to `dice: 1d6+4`. There’s an additional `dice: 1d6<=1` chance that a force field completely surrounds (above and below ground) an area; otherwise it simply rises to a height of `dice: 1d100` feet.


21-40. Illusory images or terrain should be treated as spells such as hallucinatory terrain, massmorph, or other illusion spells. Allow those passing through the illusion to roll `dice: 4d6` and compare the result to their Intelligence score. If the result is equal to or less than their score they are able to determine that there is an illusion. Illusions are the result of 


| dice: 1d6 |                                                              |
| --------- | ------------------------------------------------------------ |
| 1-2       | a spell,                                                     |
| 3-4       | a device or item,                                            |
| 5         | the influence of a powerful individual/planar connection, or |
| 6         | something else.                                              |
^IllusionOrigin

Treat the illusion as if it were a spell of level `dice: 1d8+1`.

41-60. Magical walls are just that: barriers created by such spells as wall of stone, wall of fire, etc., or potentially other spells such as acid fog, cloudkill, etc.

61-80. Zones of repulsion are invisible barriers that are otherwise treated as force fields, except they can be crossed. Once inside, an affected individual must make a saving throw against spells for every turn spent inside or be compelled to leave by the fastest means possible. Zones of repulsion have only a `dice: 1d6 <=1` chance of affecting *all* creatures that enter. Otherwise, roll below to determine what manner of creatures are affected:

39-table-1.md

| dice: 1d100 | Result                                           |
|:----------- |:------------------------------------------------ |
| 1-20        | Living creatures                                 |
| 21-40       | Unliving creatures                               |
| 41-46       | Undead                                           |
| 47-52       | Constructs                                       |
| 53-58       | Dragons                                          |
| 59-64       | Animals                                          |
| 65-70       | Elementals                                       |
| 71-76       | Fey                                              |
| 77-82       | Demons (1-3)/Angels (4-6)                        |
| 83-88       | Humans                                           |
| 89-94       | Humanoids                                        |
| 95-00       | Other (lycanthropes, a specific alignment, etc.) |
^RepulsionTarget

There’s a further `dice: 1d6<=1` chance that a specific creature type is affected by the barrier (goblins, rather than all humanoids).

Barriers can be overcome or avoided through spells, clever thinking, or simple brute force or ignorance. Labor can be used to clear a forest of hampering underbrush or to build a bridge across a ravine, as a permanent solution. Powerful magics may be needed to permanently eliminate other barriers, both magical and mundane.

### Resources

Whether abandoned mines, stands of valuable timber, patches of herbs or vast herds of animals, resources are anything that can be sold or used by the adventurers in their travels, usually in mercantile pursuits. Note that this section includes only resources that are immediately obvious – veins of precious metals unexposed to the air, mushrooms buried deep in forbidden dungeons and so forth are not included in this section.

This section makes use of the rules for generating additional resources found in the Domain Building book (starting on p. 26), as well as the Trade Goods tables on p. 38 of that supplement. When a resource result comes up use those rules to determine what general category the resource falls into and how valuable it is.

This section provides some additional rules for determining the exact type of resource that is present. The rules from Domain Building presume that resources have the same relative value based upon category. This is obviously not true if the size of the resource is the same: gold is far more valuable (typically) than copper, if found in the same quantity. The obvious remedy is to assume that the volume of the resource is different, even though it may take the same amount of time to extract it. This is something that will have to be abstracted by the Referee.

With each resource found there’s a 1 in 20 chance that it is exceptional, worth (1-3) 25% more, (4-5) 50% more, (6-7) 75% more, or (8) 100% more than the base value. This added value will be due to either exceptional purity, appearance, or other intrinsic property. It is up to the Referee to determine what the reason for the increased value is. Perhaps a vein of granite is more durable than normal, and structures built using it have more structural hit points. Or a vein of marble may have an unusual coloration, sought after by master sculptors.




40-table-1.md

| d20   | Result                                               |
|:----- |:---------------------------------------------------- |
| 1-3   | Animal, game [[#Animal, Game]]                       |
| 4-6   | Animal, livestock [[#Animal, livestock]]             |
| 7-8   | Mineral, quarried [[#Mineral Quarried]]              |
| 9-10  | Mineral, mined [[#Ore, mined]]                       |
| 11-15 | Vegetable, agricultural [[#Vegetable, agricultural]] |
| 16-20 | Vegetable, industrial [[#Vegetabel, industrial]]     |

#### Animal, Game
These are naturally occurring, wild animal resources that can be used for meat, fur, hides, or other similar products. They could also represent wild animals such as horses that are captured to be trained as mounts.

This section is divided into broad terrain and climate types. It seeks to provide a basic selection of typical animals to use, and not provide a thorough list of all the potential animals that can be found.


MULTIPLE
41-table-1.md

| dice: 1d12 | Forest                                        |
| ---------- |:--------------------------------------------- |
| 1          | Deer                                          |
| 2          | Elk                                           |
| 3          | Squirrel                                      |
| 4          | Rabbit                                        |
| 5          | Boar                                          |
| 6          | Bear                                          |
| 7          | Fox                                           |
| 8          | Wolf                                          |
| 9          | Quail                                         |
| 10         | Turkey                                        |
| 11         | Other, by terrain                             |
| 12         | Magical creature, add +1d10x10% to base price |



| dice: 1d12 | Swamp                                         |
| ---------- |:--------------------------------------------- |
| 1          | Deer                                          |
| 2          | Beaver                                        |
| 3          | Otter                                         |
| 4          | Alligator                                     |
| 5          | Snake                                         |
| 6          | Turtle                                        |
| 7          | Frog                                          |
| 8          | Crayfish                                      |
| 9          | Duck                                          |
| 10         | Clams                                         |
| 11         | Other, by terrain                             |
| 12         | Magical creature, add +1d10x10% to base price |



| Unnamed: 0 | Mountain                                      |
| ---------- |:--------------------------------------------- |
| 1          | Goat                                          |
| 2          | Hare                                          |
| 3          | Bear                                          |
| 4          | Bobcat                                        |
| 5          | Fox                                           |
| 6          | Wolf                                          |
| 7          | Squirrel                                      |
| 8          | Elk                                           |
| 9          | Turkey                                        |
| 10         | Quail                                         |
| 11         | Other, by terrain                             |
| 12         | Magical creature, add +1d10x10% to base price |

| Unnamed: 0 | Desert Badlands                               |
| ---------- |:--------------------------------------------- |
| 1          | Goat                                          |
| 2          | Hare                                          |
| 3          | Sheep                                         |
| 4          | Bison                                         |
| 5          | Auroch                                        |
| 6          | Camel                                         |
| 7          | Fox                                           |
| 8          | Wolf                                          |
| 9          | Pheasant                                      |
| 10         | Grouse                                        |
| 11         | Other, by terrain                             |
| 12         | Magical creature, add +1d10x10% to base price |

| Unnamed: 0 | Plains                                        |
| ---------- |:--------------------------------------------- |
| 1          | Deer                                          |
| 2          | Zebra                                         |
| 3          | Rhino                                         |
| 4          | Giraffe                                       |
| 5          | Hare                                          |
| 6          | Bison                                         |
| 7          | Fox                                           |
| 8          | Groundhog                                     |
| 9          | Grouse                                        |
| 10         | Quail                                         |
| 11         | Other, by terrain                             |
| 12         | Magical creature, add +1d10x10% to base price |


| Unnamed: 0 | Hills                                         |
| ---------- |:--------------------------------------------- |
| 1          | Deer                                          |
| 2          | Hare                                          |
| 3          | Boar                                          |
| 4          | Bear                                          |
| 5          | Fox                                           |
| 6          | Wolf                                          |
| 7          | Groundhog                                     |
| 8          | Sheep                                         |
| 9          | Quail                                         |
| 10         | Pheasant                                      |
| 11         | Other, by terrain                             |
| 12         | Magical creature, add +1d10x10% to base price |

| Unnamed: 0 | Salt Water                                    |
| ---------- |:--------------------------------------------- |
| 1          | Crab                                          |
| 2          | Eel                                           |
| 3          | Mussel                                        |
| 4          | Dolphin                                       |
| 5          | Whale                                         |
| 6          | Sea lion                                      |
| 7          | Sharks                                        |
| 8          | Octopus                                       |
| 9          | Tuna                                          |
| 10         | Gull                                          |
| 11         | Other, by terrain                             |
| 12         | Magical creature, add +1d10x10% to base price |


| Unnamed: 0 | Fresh Water                                   |
| ---------- |:--------------------------------------------- |
| 1          | Beaver                                        |
| 2          | Otter                                         |
| 3          | Crocodile                                     |
| 4          | Clams                                         |
| 5          | Trout                                         |
| 6          | Bass                                          |
| 7          | Gar                                           |
| 8          | Eel                                           |
| 9          | Goose                                         |
| 10         | Duck                                          |
| 11         | Other, by terrain                             |
| 12         | Magical creature, add +1d10x10% to base price |


| Unnamed: 0 | Jungle                                        |
| ---------- |:--------------------------------------------- |
| 1          | Monkey                                        |
| 2          | Water buffalo                                 |
| 3          | Capybara                                      |
| 4          | Pig                                           |
| 5          | Cougar                                        |
| 6          | Elephant                                      |
| 7          | Snake                                         |
| 8          | Hippo                                         |
| 9          | Parrot                                        |
| 10         | Toucan                                        |
| 11         | Other, by terrain                             |
| 12         | Magical creature, add +1d10x10% to base price |

#### Animal, livestock

Livestock are domestic animals that are raised for meat, furs, or work. These can be represented as actual existing animal stock (which implies there is something *in* the hex raising and caring for them), or the potential for such resources to exist; grasslands that are ideal for cattle or sheep, for instance.

Livestock animals include . . .



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

#### Mineral Quarried

There’s a base 1-3 in 6 chance that a resource of this type has previously been discovered and has been partially quarried or mined when it is encountered. This chance is decreased by 1 in Wilderness hexes and increased by 1 in Civilized hexes.  This does not affect the value of the resource, but obviously makes it more apparent and immediately accessible.

If the resource has previously been discovered there’s a base 1-3 in 6 chance it is currently being worked. This chance is increased by 1 for Civilized hexes and decreased by 1 for Wilderness hexes.

If the resource has not been discovered the vein will be found . . .

42-table-2.md

| d100   | Result                   |
|:-------|:-------------------------|
| 1-20   | Above ground and visible |
| 21-40  | 1d4×5 feet underground   |
| 41-60  | 1d4×10 feet undergound   |
| 61-80  | 2d8×20 feet underground  |
| 81-100 | 3d10×50 feet underground |


The further a resource is underground the more difficult it is to find, and the more labor it takes to expose it. Strip mining or quarrying costs 400 gp per 20,000 cubic feet of earth removed. However, the surface opening needs to be the same diameter as the depth. A 10’ depth requires a perimeter of 10’×10’ (1,000 cubic feet of excavated material). A 30’ depth requires a perimeter of 30’×30’ (27,000 cubic feet).

Mining tunnels cost 500 gp per ten feet of depth. This assumestunnels10’×10’,reinforcedasneededtoprevent collapses. Mining tunnels deeper than 100 feet cost 750 gp per 10’ of depth.

Following are some types of stone that can be quarried.

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


Quarried minerals, once extracted, do not have to be smelted or processed to use, although some of them certainly can be (sand, for instance, can be heated and turned into glass). They do not need to be chemically refined or altered in order to be useful, however.

Minerals are not part of the Trade Good table (p. 38 of Domain Building), so they have been added here:

Added Trade Goods

42-table-1.md

| Unnamed: 0        | Load     | Enc/load   | Base Price   |
|:------------------|:---------|:-----------|:-------------|
| Quarried Minerals | 1 box    | 10,000 cn  | 150 gp       |
| Stone             | 1 pallet | 5,000 cn   | 1,000 gp     |

###### Quarried Minerals (common). 

These include common materials that are quarried for alchemical usage (such as gypsum) or for base building materials: Chalk, Clay, Gabbro, Gypsum, Sand, Slate.

###### Stone (rare). Coal, Coquina, Granite, Limestone, Marble*, Sandstone.

*marble has a base price of 1,500 gp per load.

#### Ore, mined

Valuable minerals are less likely to be visible than quarried rocks. Use the same table, above, to determine the depth at which the resource is found, adding 5 to the roll for metal and 10 for gemstones.

Mined minerals have the same chances as quarried stone to be exceptional. Mined ore will contain either (1-4) minerals or (5-6) gemstones (putting aside the fact that gemstones are, in fact, minerals).

Following are some examples of mined minerals.


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



Mined minerals must be smelted. Depending on the mineral and how far it must travel to its destination it can either be smelted at the mine or shipped back to civilization and then smelted.

Smelters cost 5,000 gp to build. Once complete, a smelter can process a total of 50 gp worth of ore per day. A smelter requires a minimum crew of four workers (one trained worker making 50 gp per month and three laborers making three gp a month) and costs 2 gp per day in raw materials per day of operation. Optionally, smelters designed to purify rare or magical metals may be more expensive to build and/or run than normal smelters.

The starting weight of mined ore is extrapolated from the finished weight of refined ore found on p. 38 of the Domain Building supplement. There are two types of refined ore: common and precious. Refer to the following tables to determine the weight multipliers for each material (note that these are abstracted figures meant to provide general guidelines, and do not hew directly to real-world examples).


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

Ex. Copper, with a multiplier of 2, requires 100 cn of raw ore to yield 50 cn of refined material. Lead, with a multiplier of 1.1, requires 55 cn to yield the same amount

Precious Ore. Base value of 1.5 gp/1 cn
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


Alchemical metals. These have a base value of 1d6 gp per cn and a multiplier of ×1d6

Special/magical metals. These have a base value of 2d6 per cn and a multiplier of ×1d8

Ex. Gold, with a multiplier of 1.25, requires 1.25 cn of raw material to yield 1 cn of pure gold.

Gems require no smelting and are most often mined in the same fashion as metal. They are found in the rough, however, and require work to cut and polish.


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


Wholesale gemstone prices can be found on p. 38 of Domain Building, as follows:

-   􏰀  Semi-precious stones cost a base of 2 gp per cn of weight.
    
-   􏰀  Precious stones cost a base of 60 gp per cn of weight.
    
    These are abstracted numbers. They can be modified based upon the stone, if desired, with the following modifiers:

Semi-precious stones
    
    􏰀 Agate, quartz, turquoise ×.5  
    􏰀 Jacinth, jasper, onyx ×1  
    􏰀 Amber, amethyst, coral, garnet, jade ×1.5
    
    Ex. An agate mine yields uncut stones that are worth 1 gp per cn of weight. A jade mine yields uncut jade worth 3 gp per cn

Precious stones

􏰀 Aquamarine, pearl, topaz ×.5 􏰀 Carbuncle, opal ×.1  
􏰀 Emerald, ruby, sapphire ×1.5 􏰀 Diamond ×2

􏰀 Magical, unique ×5

Ex. An aquamarine mine yields uncut stones worth 30 gp per cn. A diamond mine yields uncut stones worth 120 gp per cn.


#### Vegetable, agricultural

Plant resources used for food. This can be food that exists naturally in the area or crops that are currently being grown by sentient creatures. This, of course, suggests that there is someone currently growing the plants, although it is certainly possible to find abandoned agricultural operations: orchards abandoned and growing wild, or gardens left untended to go to seed, etc.

Agricultural resources are divided into two categories: cultivated and wild. Cultivated plants are tended and harvested on a regular basis; wild plants grow wild, as the name implies, without caretaking, but may certainly be harvested on a regular basis by those living nearby (both humanoids and animals).

There’s a 1-3 in 6 chance that the resource will be wild; otherwise it will be cultivated. This chance increases by 1 in Wilderness hexes and decreases by 1 in Civilized hexes. There’s a further 1 in 6 chance that cultivated resources have been abandoned in the past 1d12 years. This chance increases by 1 in Wilderness hexes.


Cultivated

The following plants are those commonly cultivated by Man. Roll 1d10 to determine what kind of cultivated plant is being grown.

1-4. Grain. Staple crops for many societies, grains are typically cultivated in large amounts, requiring large fields, open spaces, and plenty of labor to harvest. Some grains grow better in different climates; rye is typically a cold weather crop, rice prefers wet climates, etc.

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


5-7. Vegetables. Vegetables are typically grown in smaller quantities than grains and used mostly as supplemental crops rather than primary meal sources. This list is not inclusive of all vegetables.

45-table-1.md

45-table-4.md

| d100  | Result          |
|:----- |:--------------- |
| 1-4   | Artichokes      |
| 5-8   | Asparagus       |
| 9-12  | Bamboo          |
| 13-16 | Beans           |
| 17-20 | Beets           |
| 21-24 | Broccoli        |
| 25-28 | Cabbage         |
| 29-32 | Carrots         |
| 33-36 | Cassava         |
| 37-40 | Cucumber        |
| 41-44 | Edamame         |
| 45-48 | Eggplant        |
| 49-52 | Garlic          |
| 53-56 | Gourd           |
| 57-60 | Lettuce         |
| 61-64 | Onions          |
| 65-71 | Other           |
| 72-75 | Pepper          |
| 76-79 | Peas            |
| 80-83 | Potato          |
| 84-87 | Spinach         |
| 88-91 | Squash          |
| 92-95 | Turnip          |
| 96-99 | Yam             |
| 100   | Magical/Special |


8-9. Fruit. The below are a list of some more common fruits, as well as the general category of fruit they belong to.


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

Nuts/Spices/Other. The most rare, and most valuable, category of agricultural vegetables. Spices use the spice category on the Rare Trade Goods table, nuts and other vegetables have their base value increased by 2d6×10%.

46-table-2.md

| d100  | Result                                         |
|:----- |:---------------------------------------------- |
| 1-4   | Almond                                         |
| 5     | Cardamom                                       |
| 6-9   | Cashew                                         |
| 10-13 | Chestnut                                       |
| 14    | Cacao bean                                     |
| 15    | Clove                                          |
| 16    | Coconut                                        |
| 17    | Coffee                                         |
| 18-20 | Dill                                           |
| 21-24 | Hazelnut                                       |
| 25    | Paprika                                        |
| 26-29 | Pecan                                          |
| 30-31 | Peppercorns                                    |
| 32-33 | Marijuana                                      |
| 3436  | Mint                                           |
| 37-39 | Mushroom, oyster                               |
| 40-41 | Mushroom, shitake                              |
| 42    | Mushroom, psilocybin                           |
| 43-44 | Nutmeg                                         |
| 45-61 | Other                                          |
| 62-65 | Peanut                                         |
| 66-69 | Pecan                                          |
| 70-72 | Pine-nut                                       |
| 73-75 | Pistachio                                      |
| 76-77 | Poppy                                          |
| 78-81 | Oregano                                        |
| 82-84 | Rosemary                                       |
| 85    | Saffron                                        |
| 86-89 | Thyme                                          |
| 90-92 | Tobacco                                        |
| 93-94 | Turmeric                                       |
| 95    | Vanilla                                        |
| 96-99 | Walnut                                         |
| 100   | Magical/Special.  Add  2d6×10%  to base price. |


Wild

The following plants can be found growing wild and have agricultural, alchemical, or medicinal uses. Use the Spice row on the Rare Trade Goods table.




46-table-1.md

| d100  | Result                                      |
|:----- |:------------------------------------------- |
| 1-4   | Aloe vera                                   |
| 5-8   | Angelica                                    |
| 9-12  | Arnica                                      |
| 13-16 | Belladonna                                  |
| 17-20 | Burdock                                     |
| 21-24 | Cohosh                                      |
| 25-28 | Comfrey                                     |
| 29-32 | Coneflower                                  |
| 33-36 | Dandelion                                   |
| 37-40 | Foxglove                                    |
| 41-44 | Ginseng                                     |
| 45-48 | Hawthorn                                    |
| 49-52 | Horsetail                                   |
| 53-56 | Marshmallow                                 |
| 57-60 | Mushrooms                                   |
| 61-64 | Neem                                        |
| 65-68 | Nettles                                     |
| 69-78 | Other                                       |
| 79-82 | Rosehips                                    |
| 83-86 | Seaweed                                     |
| 87-91 | Snakeroot                                   |
| 92-95 | Thistle                                     | 
| 96-99 | Wolfsbane                                   |
| 100   | Magic/Special.  Add  1d8×10% to base price. |

#### Vegetabel, industrial
Plant resources that are used for building, construction, etc., as well as other uses such as fibers for ropes and clothing. These are divided into three basic categories: (1-3) Basic, (4-5) Structural, (6) Luxury.

Basic. This category includes all vegetable goods for textiles, paper, and basic construction work; firewood, scaffolding, lath, etc.


46-table-3.md

| d100  | Result                                                                                                                                  |
|:----- |:--------------------------------------------------------------------------------------------------------------------------------------- |
| 1-5   | Bamboo                                                                                                                                  |
| 6-10  | Birch-bark                                                                                                                              |
| 11-15 | Cotton                                                                                                                                  |
| 16-20 | Flax                                                                                                                                    |
| 21-25 | Grasses (for basketry or similar)                                                                                                       |
| 26-30 | Hemp                                                                                                                                    |
| 31-35 | Jute                                                                                                                                    |
| 36-40 | Other                                                                                                                                   |
| 41-45 | Palm                                                                                                                                    |
| 46-50 | Papyrus                                                                                                                                 |
| 51-55 | Seaweed (reroll if not appropriate)                                                                                                     |
| 56-60 | Sisal                                                                                                                                   |
| 61-65 | Straw                                                                                                                                   |
| 66-99 | Wood  (roll  on  the  (1-4)  Structural or (5-6) Luxury table below, but use the  Wood,  Common  row  on  the Common Trade Goods table) |
| 100   | Magical/Special. Add 5d10×10% to base price.                                                                                            |

Structural. Includes trees and plants used for construction, from buildings to other structures, carts, wagons, boats, etc. Use the Wood, Common row on the Common Trade Goods table but with a base cost of 250 gp.


47-table-4.md

| d100  | Result                                            |
|:----- |:------------------------------------------------- |
| 1-4   | Ash                                               |
| 5-8   | Alder                                             |
| 9-12  | Birch                                             |
| 13-16 | Cedar                                             |
| 17-20 | Cherry                                            |
| 21-24 | Chestnut                                          |
| 25-28 | Cottonwood                                        |
| 29-32 | Eucalyptus                                        |
| 33-36 | Fir                                               |
| 37-40 | Ginkgo                                            |
| 41-44 | Hickory                                           |
| 45-48 | Larch                                             |
| 49-52 | Maple                                             |
| 53-56 | Oak                                               |
| 57-67 | Other                                             |
| 68-71 | Pine, yellow                                      |
| 72-75 | Poplar                                            |
| 76-79 | Purpleheart                                       |
| 80-83 | Redwood                                           |
| 84-87 | Spruce                                            |
| 88-91 | Sycamore                                          |
| 92-95 | Yellow-wood                                       |
| 96-99 | Yew                                               |
| 100   | Magical/Special.  Add  1d8×10%  to the base cost. |


100. Luxury. Rare or exotic trees used for furniture, high- end woodworking, lavish details in royal dwellings, etc.


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

### Hazard


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

### Terrain

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

| dice: 1d5 |                                    |
| --------- | ---------------------------------- |
| 1         | `dice: [[Fill#^TerrainForest]]`    |
| 2         | `dice: [[Fill#^TerrainHills]]`     |
| 3         | `dice: [[Fill#^TerrainMountains]]` |
| 4         | `dice: [[Fill#^TerrainWetlands]]`  |
| 5         | `dice: [[Fill#^TerrainArid]]`      |
| 6         | `dice: [[Fill#^TerrainFlat]]`      |
^TerrainType


| 1d8 | Forest            |
| --- | ----------------- |
| 1   | Light, Coniferous |
| 2   | Heavy, Coniferous |
| 3   | Light, Deciduous  |
| 4   | Heavy, Deciduous  |
| 5   | Light, Mixed      |
| 6   | Heavy Mixed       |
| 7   | Rainforest        |
| 8   | Other             |
^TerrainForest


| 1d8 | Hills               |
| --- | ------------------- |
| 1   | Hills, Grasslands   |
| 2   | Hills, Barren       |
| 3   | Hills, Forested     |
| 4   | Hills, Shrub        |
| 5   | Hills, Jungle       |
| 6   | Hills, Transitional |
| 7   | Hills, Lone         |
| 8   | Other               |
^TerrainHills


| 1d8 | Mountains                   |
| --- | --------------------------- |
| 1   | Muntains, Small-Barren      |
| 2   | Mountains, Small-Forested   |
| 3   | Mountains, Tall-Barren      |
| 4   | Mountains, Tall-Forested    |
| 5   | Mountains, Tall-Snow Capped |
| 6   | Volcano                     |
| 7   | Plateau                     |
| 8   | Other                       |
^TerrainMountains


| 1d8 | Wetlands |
| --- | -------- |
| 1   | Bog      |
| 2   | Marsh    |
| 3   | Swamp    |
| 4   | Jungle   |
| 5   | River    |
| 6   | Moor     |
| 7   | Fungal   |
| 8   | Other    |
^TerrainWetlands


| 1d8 | Arid            |
| --- | --------------- |
| 1   | Desert, Cold    |
| 2   | Desert, Hot     |
| 3   | Desert, Coastal |
| 4   | Desert, Rocky   |
| 5   | Badlands        |
| 6   | Steppes         |
| 7   | Flats           |
| 8   | Other           |
^TerrainArid


| 1d8 | Flat       |
| --- | ---------- |
| 1   | Prairie    |
| 2   | Grazing    |
| 3   | Farmland   |
| 4   | Shrublands |
| 5   | Savanna    |
| 6   | Flats      |
| 7   | Tundra     |
| 8   | Other      |
^TerrainFlat


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