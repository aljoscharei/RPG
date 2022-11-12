---
Name: 
Ini: 
Hp: 
Dmg: 0
Defense: 
Armor: 
AttackAttr: 
Weapon: 
---
[[202202111122 Bestiary MOC]]
[[202108140221 RPG MOC]]
[[202201061059 Ruins of symbaroum MOC]]
[[outfile]]





```dataviewjs
var thisFight = dv.pages("#thisFight")
dv.header(1,"This Fight, to include tag Note with #thisFight")
dv.table(
["Link", "Ini","Hp","Dmg","Defense", "Armor", "AttackAttr.", "Weapon"],
thisFight
.sort(k => k.Ini,'desc')
.map(k => [k.file.link, k.Ini,k.hp, k.Dmg,k.Defense, k.Armor, k.AttackAttr, k.Weapon])

)
```
- irgenwie will ich noch spalten in denen ich abkreuzen kann, wer schon welche art von action gehabt hat (action, move, bonus action, free action)  [[5e order of combat]]
- YAML:
	- wenn man im stat block enter drückt, dann sind die leerzeichen Tabs, YAML benötigtaber immer: SPACE SPACE MINUS SPACE. Wenn anders ist YAML invalid und kann von Statblock nicht gelesen werden
	- habe parallel reading and editing mode offen, dann siehst du sofort wenn etwas invalid ist.


[[202201072142 symbaroum MOC]]
[[Ruins GM Index]]
[[202201101101 NPC MOC]]
[[Ruins of Symbaroum Monster Features MOC]]
[[Symbaroum 5e Monster Features]]
[[Symbaroum Random Encounter Tables]]


# 5e Stats 
https://docs.google.com/spreadsheets/d/16jzFlPxWvfFZVtGBylr7Vc8fKc1qqYcunjOaV36mPys/edit#gid=776794522&range=A810
## 3 Round Combat Plan
Action oriented monsters:  
- In position invisibility  
- Get out of a bad spot, of being ganged up thunderwave, misty step thinderstep  
- Climax sth that wishes pcs that they never met him  
	- Explode or free attacks against anyone   
- [[Keith Ammann - The Monsters Know What They’re Doing-DMs Guild.pdf]]
- [[Encounters MOC]]

# Encounter Table

```dataviewjs
var thisFight = dv.pages("#Enc1")
dv.header(1,"Random Combat Encounter, to include tag Note with #Enc1")
dv.table(
["Link", "Ini","Hp","Dmg","Defense", "Armor", "AttackAttr.", "Weapon"],
thisFight
.sort(k => k.Ini,'desc')
.map(k => [k.file.link, k.Ini,k.hp, k.Dmg,k.Defense, k.Armor, k.AttackAttr, k.Weapon])

)
```


```encounter
name: PCs
creatures:
 - 1: Rojazz
 - 1: Paco
 - 1: Variol
 - 1: Cult Fanatic
 - 3: Cultist
 - 2: Giant Centipede
```




```encounter-table
name: Example 1
creatures:
 - Hobgoblin
 - 3: Goblin

---

name: Example 2
creatures:
 - 3: Hobgoblin
 - Goblin

```


[[Symbaroum Random Encounter Tables]]

- Homebrew
	- [[Symbaroum Monster Tattooed Barbarian Warrior]]
	- [[Symbaroum Monster Symbolist]]

- Townsfolk
	- [[Symbaroum Monster Artisan CR 1]]
	- [[Symbaroum Monster Drug Peddler]]
	- [[Symbaroum Monster Drunkard]]
	- [[Symbaroum Monster Guard Dog]]
	- [[Symbaroum Monster Innkeeper]]
	- [[Symbaroum Monster Medicus]]
	- [[Symbaroum Monster Noble Brat]]
	- [[Symbaroum Monster Self-taught Withch hunter]]

- Trolls
	- [[Symbaroum Monster Arch Troll]]
	- [[Symbaroum Monster Liege Troll]]
	- [[Symbaroum Monster Mountain Troll]]
	- [[Symbaroum Monster Pale Crawler]]
	- [[Symbaroum Monster Famished Rage Troll]]
	- [[Symbaroum Monster Group-livin Rage Troll]]

- Abominations
	- [[Symbaroum Monster Blight-Born Aboar]]
	- [[Symbaroum Monster Blight-born Elk]]
	- [[Symbaroum Monster Blight-born Fairies]]
	- [[Symbaroum Monster Blight-Born Human]]
	- [[Symbaroum Monster Blight Worm]]
	- [[Symbaroum Monster The Black Plague Termites]] 
	- [[Symbaroum Monster Chasm Stag]]
	 - [[Symbaroum Monster Primal Blight Beast]]
	 - [[Symbaroum Monster The Wily]]
- Amphibians Aquatics
	- [[Symbaroum Monster Cave Ray]]
	- [[Symbaroum Monster Drilling Leech]]
	- [[Symbaroum Monster Hammer Eel]]
	- [[Symbaroum Monster Nipper]]
	- [[Symbaroum Monster Skullan]]
	- [[Symbaroum Monster Vapaya]]
- Flora
	- [[Symbaroum Monster Brimstone Oak]]
	- [[Symbaroum Monster Kelder]]
	- done[[Symbaroum Monster Killer Shrub]]
- Herbivores
	- [[Symbaroum Monster Darak]]
	- [[Symbaroum Monster Moose]]
	- [[Symbaroum Monster Rock Buck]]

- Predators
	- [[Symbaroum Monster Aboar]]
	- [[Symbaroum Monster Marlit]]
	-  [[Symbaroum Monster Sly River Hunter]]
	- [[Symbaroum Monster Baiagorn]]
	- [[Symbaroum Monster Beamon]]
	- [[Symbaroum Monster Blood cat]]
	- [[Symbaroum Monster Ferber]]
	- [[Symbaroum Monster Fey Beast]]
	- [[Symbaroum Monster Garoug]]
	- [[Symbaroum Monster Hunger Wolf]]
	- [[Symbaroum Monster Jakaar, battle-trained]]
	- [[Symbaroum Monster Jakaar]]
	- [[Symbaroum Monster Kanaran]]flin
	- [[Symbaroum Monster Kotka]]
	- [[Symbaroum Monster Mare Cat]]
	- [[Symbaroum Monster Mosey Munk]]
	- [[Symbaroum Monster Orahaug]]
	- [[Symbaroum Monster Stone Boar]]
	- [[Symbaroum Monster Vearon Löwenechse]]

- Spiders
	- [[Symbaroum Monster Etterherd]]
	- [[Symbaroum Monster Fray Spider]]
	- [[Symbaroum Monster Hunting Spider]]
	- [[Symbaroum Monster Spider Queen]]
	- [[Symbaroum Monster Tricklesting]]
	- [[Symbaroum Monster Xanatha]]
	
- Undead
	- [[Symbaroum Monster Crypt Lord]]
	- [[Symbaroum Monster Cryptwalker]]
	- [[Symbaroum Monster Dragoul Zombie]]
	- [[Symbaroum Monster frostlight alt dmg resolute and d4 temp corr res save oder zwangshandlung Geisterecho]]
	- [[Symbaroum Monster Lostling Possession]]
	- [[Symbaroum Monster Necromage]]
	- [[Symbaroum Monster Snow wraith]]
	- [[Symbaroum Monster Wraith]]
- Winged Creatures
	- [[Symbaroum Monster Blaze Bug]]
	- [[Symbaroum Monster Crystal Flies]]
	- [[Symbaroum Monster Dragon Fly]]
	- [[Symbaroum Monster Hornet]]
	- [[Symbaroum Monster Raskaal]]
	- [[Symbaroum Monster Violing]]
	- [[Symbaroum Monster Wraith Owl]]

- Champions of Prios
	- [[Symbaroum Monster Black Cloak]]
	- [[Symbaroum Monster Experienced Black Cloak]]
	- [[Symbaroum Monster Flagellant]]
	- [[Symbaroum Monster Liturg]]
	- [[Symbaroum Monster Templar]]
	- [[Symbaroum Monster Theurg]]
	- [[Symbaroum Monster The Whip of Prios]]

- Elves
	- [[Symbaroum Monster Spring Elf]]
	- [[Symbaroum Monster Early Summer Elf]]
	- [[Symbaroum Monster Late Summer Elf]]
	- [[Symbaroum Monster Autumn Elf]]

- Lords of Ambria
	- [[Symbaroum Monster Bailiff]]
	- [[Symbaroum Monster Knight]]
	- [[Symbaroum Monster Lord or Lady]]
	- [[Symbaroum Monster Squire]]

- Ordo Magica
	- [[Symbaroum Monster Adept of Ordo Magica]]
	- [[Symbaroum Monster Artifact Crafter]]
	- [[Symbaroum Monster Magistrate CR too high]]
	- [[Symbaroum Monster Master of the Order]]
	- [[Symbaroum Monster Novice of the Order]]
	- [[Symbaroum Monster Panzer Alchemist]]
	- [[Symbaroum Monster Ritual Master]]

- Outsiders
	- [[Symbaroum Monster Cult Follower]]
	- [[Symbaroum Monster Cult Leader]]
	- [[Symbaroum Monster Fortune Hunter]]
	- [[Symbaroum Monster Pickpocket]]
	- [[Symbaroum Monster Plunderer]]
	- [[Symbaroum Monster Robber]]
	- [[Symbaroum Monster Robber Chief]]
	- [[Symbaroum Monster Thug]]

- People of Davokar
	- [[Symbaroum Monster Goblin Tribesman]]
	- [[Symbaroum Monster Goblin Chieftain]]
	- [[Symbaroum Monster Goblin Shaman]]
	- [[Symbaroum Monster Goblin Warrior]]
	- [[Symbaroum Monster Monster Hunter]]
	- [[Symbaroum Monster Queens Ranger]]
	- [[Symbaroum Monster ranger captain]]
	- [[Symbaroum Monster Barbarian Village guard]]
	- [[Symbaroum Monster Village Barbarian warrior]]
	- [[Symbaroum Monster Village Witch]]
	- [[Symbaroum Monster Wilderness Guide Barbarian or Goblin]]
	- [[Symbaroum Monster Witch - Keeper]]

- People of the Queen
	- [[Symbaroum Monster Archer]]
	- [[Symbaroum Monster Farmhand]]
	- [[Symbaroum Monster Horse]]
	- [[Symbaroum Monster Horse, battle-trained]]
	- [[Symbaroum Monster Infantryman]]
	- [[Symbaroum Monster Officer]]
	- [[Symbaroum Monster Pansar]]
	- [[Symbaroum Monster Pikeman]]
	- [[Symbaroum Monster Queen s Spy]]
	- [[Symbaroum Monster Sapper]]
- 

	- [[Symbaroum Monster Throne Beast Krötenstier]]
	- [[Symbaroum Monster Krazaragas der Hüter]]
	- [[202203292238 Monster Spinne Goldene Prophetin Sonne Skullbiter Queen]]
	- [[Symbaroum Monster Oroke]]
	- [[Symbaroum Monster Aloena]]
	- [[Symbaroum Monster Staubmenschen Staubläufer]]
	- [[Symbaroum Monster Etterherd]]
	- [[Symbaroum Monster Alahara]]

	- [[Symbaroum Monster der Untote Lenn]]
	- [[Symbaroum Monster Gorak]] 
	- [[Symbaroum Monster Baumelo-Odako]]
	- [[Symbaroum Monster Morcai  Punk mit Inselfrisur seine Handlanger]]
	- [[Symbaroum Monster Tivos sein Handlanger Roter Backenbart]]
	- [[Symbaroum Monster Lymbra seine Handlangerin verrhärmte Frau]]
	- [[Symbaroum Monster Terr the Psychic]]
	- [[Symbaroum Monster The Skull]]





- Full page
	- [[Symbaroum Monster Arach Exalted]]
	- [[Symbaroum Monster Ettermite]]
	- [[Symbaroum Monster Arach Poisoner]]
	- [[202201311237 Monster Lasifor Angathal Taar Spinnenlich]]
	- [[Symbaroum Monster Menandra Na ya]]
	- [[Symbaroum Monster glowing Guard]]
	- [[Symbaroum Monster creeping darkness]]
	- [[Symbaroum Monster bestiaal clawing fighter]]
	- [[Symbaroum Monster Bestiaal - Glint Carrier]]
	- [[Symbaroum Monster Bestiaal Winged Hunter]]
	- [[Symbaroum Monster Coloss]]
	- [[Symbaroum Monster Corrupted Nature Intruder Demon]]
	- [[Symbaroum Monster Darkling Hunter]]
	- [[Symbaroum Monster Darkling Leader]]
	- [[Symbaroum Monster Death Prince]]
	- [[Symbaroum Monster lindwurm]]
	- [[Symbaroum Monster Drakworm]]
	- [[Symbaroum Monster Dragon]]
	- [[Symbaroum Monster Glimmer]]
	- [[Symbaroum Monster Glint Goldkäfer]]
	- [[Symbaroum Monster Glint-Carrier Aboar]]
	- [[GM_FlohFelixAljoscha/Symbaroum Monsters/Symbaroum Monster Glint-Carrier, Guard Warrior]]^4de6c5
	- [[Symbaroum Monster Gwann Slaughterer]]
	- [[Symbaroum Monster Gwann normal-sized]]
	- [[Symbaroum Monster Illgoblin]]
	- [[Symbaroum Monster King Toad older]]
	- [[Symbaroum Monster King Toad young]]
	- [[Symbaroum Monster Linving Thorns, Wild]]
	- [[Symbaroum Monster living Thorns, Familiar]]
	- [[Symbaroum Monster Managaal, Adult]]
	- [[Symbaroum Monster Managaal, Spawn]]
	 - [[Symbaroum Monster Neferani]]
	 - [[Symbaroum Monster Nightmare]]
	 - [[Symbaroum Monster Night Swarmers, Swarm]]
	 - [[Symbaroum Monster Night Swarmers, Murder Cloud]]
	 - [[Symbaroum Monster Ravenous Willow, Young Strangler CR 14]]
	 - [[Symbaroum Monster Ravenous Willow, old Crusher]]
	 - [[Symbaroum Monster Scorner]]
	 - [[Symbaroum Monster skullbiter hatchling]]
	 - [[Symbaroum Monster skullbiter Crusher]]
	 - [[Symbaroum Monster skullbiter Queen]]
	 - [[Symbaroum Monster Spite]]
	 - [[Symbaroum Monster Troll Shadow]]
	 - [[Symbaroum Monster Vengeful Terrain Choking Undine]]
	 - [[Symbaroum Monster Vengeful Terrain Gobble Gnome]]
	 - [[Symbaroum Monster Vengeful Terrain Hunger Fury]]
	 - [[Symbaroum Monster Vengeful Terrain Ire Sylph]]
	 - [[Symbaroum Monster World Serpent Tunneler CR 17]]
	 - [[Symbaroum Monster World Serpent Wallower CR 26]]

	- No 5e Statblock
		- [[stone_golem]]
		- [[202203292238 Monster Spinne Goldene Prophetin Sonne Skullbiter Queen]]
		- [[Symbaroum Monster Spectral Swarm]]




Monsters by CR

no statblock
[[Symbaroum Monster Xiximanter.md]]
[[Symbaroum Monster Terr the Psychic]]
[[Symbaroum Monster Staubmagier Shushushi]]
[[Symbaroum Monster Vindictive Daemon]]
[[Symbaroum Monster Vapaya]]
[[Symbaroum Monster Throne Beast Krötenstier]]
[[Symbaroum Monster Staubtausendfüßler]]
[[Symbaroum Monster Springspinne]]
[[Symbaroum Monster Cave Ray 2]]
[[Symbaroum Monster Alahara]]
[[Symbaroum Monster Oroke]]
[[Symbaroum Monster Arach Ammen]]
[[Symbaroum Monster Menandra Na ya]]
[[Symbaroum Monster Gorak]]
[[Symbaroum Monster Leogai Templer]]
[[Symbaroum Monster Morcai  Punk mit Inselfrisur seine Handlanger]]
[[Symbaroum Monster Shelob]]
[[Symbaroum Monster Baumelo-Odako]]
[[Symbaroum Monster Thorn Beasty]]
[[Symbaroum Monster Zwergenmutter]]
[[Symbaroum Monster Basilisk]]
[[Symbaroum Monster Aloena]]
[[Symbaroum Monster der Untote Lenn]]
[[Symbaroum Monster the Weaver]]
[[Symbaroum Monster Fischhexe]]
[[Symbaroum Monster Xanatha]]
[[Symbaroum Monster Eufrynda]]
[[Symbaroum Monster Hermon]]
[[Symbaroum Monster The Skull]]
[[Symbaroum Monster Servant Daemon]]
[[Symbaroum Monster Kullinan]]
[[Symbaroum Monster Godalg]]
[[Symbaroum Monster Pelurskgeist]]
[[Symbaroum Monster Lymbra seine Handlangerin verrhärmte Frau]]
[[Symbaroum Monster Knowledge Daemon]]
[[Symbaroum Monster Spectral Swarm]]
[[Symbaroum Monster Krazaragas der Hüter]]
[[Symbaroum Monster glowing Guard]]
[[Symbaroum Monster Deseba]]
[[Symbaroum Monster Schlangenkönig Gilad]]
[[Symbaroum Monster Pelurskitkönige]]
[[Symbaroum Monster Xiximutter Xiximanters Zwergenmutter]]
[[Symbaroum Monster Guardian Daemon]]
[[Symbaroum Monster Staubglob]]
[[Symbaroum Monster Archivmeister Shushush]]
[[Symbaroum Monster creeping darkness]]
[[Symbaroum Monster Tivos sein Handlanger Roter Backenbart]]
[[Players_FlohFelixAljoscha/Symbaroum Monster Flaming Servant]]


```statblock
image: [[Wikilink To Image]]
name: string
size: string
type: string
subtype: string
alignment: string
ac: number
hp: number
hit_dice: string
speed: string
stats: [number, number, number, number, number, number]
fage_stats: [number, number, number, number, number, number, number, number, number]
saves:
  - <ability-score>: number
skillsaves:
  - <skill-name>: number
damage_vulnerabilities: string
damage_resistances: string
damage_immunities: string
condition_immunities: string
senses: string
languages: string
cr: number
spells:
  - <description>
  - <spell level>: <spell-list>
traits:
  - name: <trait-name>
    desc: <trait-description>
  - ...
actions:
  - name: <trait-name>
    desc: <trait-description>
  - ...
legendary_actions:
  - name: <legendary_actions-name>
    desc: <legendary_actions-description>
  - ...
bonus_actions:
  - name: <trait-name>
    desc: <trait-description>
  - ...
reactions:
  - name: <reaction-name>
    desc: <reaction-description>
  - ...
```
