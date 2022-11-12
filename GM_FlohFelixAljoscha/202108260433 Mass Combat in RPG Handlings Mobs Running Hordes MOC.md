[[Wargame MOC]]
[[202101251048 Symbaroum DMG GM Guide]]
 [[202108260433 Mass Combat in RPG Handlings Mobs Running Hordes MOC]]
[[202202101110 5e DnD DMG Dungeon Masters Guide]] p 250
[[Ruins GM Index]]
[[Sly flourish lazy dm companion.pdf]] p 35 Running Hordes 
[[202203091103 Sly flourish lazy dm companion MOC]]


### Handling Mobs

Keeping combat moving along at a brisk pace can be difficult when there are dozens of monsters involved in a battle. When handling a crowded battlefield, you can speed up play by forgoing attack rolls in favor of approximating the average number of hits a large group of monsters can inflict on a target.

Instead of rolling an attack roll, determine the minimum d20 roll a creature needs in order to hit a target by subtracting its attack bonus from the target’s AC. You’ll need to refer to the result throughout the battle, so it’s best to write it down.

Look up the minimum d20 roll needed on the Mob Attacks table. The table shows you how many creatures that need that die roll or higher must attack a target in order for one of them to hit. If that many creatures attack the target, their combined efforts result in one of them hitting the target.

For example, eight [[orc]] surround a fighter. The orcs’ attack bonus is +5, and the fighter’s AC is 19. The orcs need a 14 or higher to hit the fighter. According to the table, for every three orcs that attack the fighter, one of them hits. There are enough orcs for two groups of three. The remaining two orcs fail to hit the fighter.

If the attacking creatures deal different amounts of damage, assume that the creature that deals the most damage is the one that hits. If the creature that hits has multiple attacks with the same attack bonus, assume that it hits once with each of those attacks. If a creature’s attacks have different attack bonuses, resolve each attack separately.

This attack resolution system ignores critical hits in favor of reducing the number of die rolls. As the number of combatants dwindles, switch back to using individual die rolls to avoid situations where one side can’t possibly hit the other.

| d20 Roll Needed | Attackers Needed for One to Hit |
| --------------- | ------------------------------- |
| 1–5             | 1                               |
| 6–12            | 2                               |
| 13–14           | 3                               |
| 15–16           | 4                               |
| 17–18           | 5                               |
| 19              | 10                              |
| 20              | 20                              |
this is the calculator for that 
#### Mob Damage Calculator
https://slyflourish.com/mob_calculator.html
this is the core function:
```js
function output(){
    var ac = parseInt(document.getElementById('ac').value);
    var amount = parseInt(document.getElementById('amount').value);
    var attack = parseInt(document.getElementById('attack').value);
    var damage = parseInt(document.getElementById('damage').value);

    if (ac - attack > 20) { var avac = 20; }
    else { var avac = ac - attack; }
    pctMonstersThatHit = (21 - avac) / 20;
    numMonstersThatHit = Math.floor(pctMonstersThatHit * amount);
    totalDamage = numMonstersThatHit * damage;

    result = numMonstersThatHit + " monsters of " + amount + " (" + Math.floor(pctMonstersThatHit * 100) + "% of total) hit for a total of " + totalDamage + " damage.</p><p>If calculating for monster saving throws, " + numMonstersThatHit + " monsters of " + amount + " (" + Math.floor(pctMonstersThatHit * 100) + "%) make their saving throw.";
    document.getElementById('result').innerHTML = result;
}
```

# Running Hordes: The Lazy Way to Run Lots of D&D Monsters

This article offers a simple system for running dozens to hundreds of monsters in your D&D battles.

## Rules Summary

-   Tally damage done to any member of the horde in a single tally. Any time that tally is higher than the hit points of a single monster, remove a monster. Round monster hit points to the nearest 5 or 10 to make the math easier.
-   Whenever the monsters attack or must make a saving throw, assume one quarter succeeds and round up or down depending on the sitation. Increase this to half if the monsters have advantage or one in ten if they have disadvantage.
-   Adjudicate areas of effect by assuming lots of members of the horde are caught in the area. Small areas hit four, medium areas like _thunder wave_ or _burning hands_ hit eight, large areas like _fireball_ or _turn undead_ hit sixteen. Huge areas like _circle of death_ hit thirty two. If the damage done by an area of effect is close to a single monster's hit points, remove the monsters if they fail the saving throw.

For a video on this topic, see my [Running Hoards Youtube video](https://www.youtube.com/watch?v=SfqcVlSnf2k).

## Epic Battles of Heroes Against Hordes

The heroes stand atop a mountain of bones with one hundred skeletons swarming in. The cleric holds her holy symbol aloft and waves of radiant energy tear through the skeletons, shattering dozens of the creatures before the rest roar in.

Our heroes stand atop the ruins of an elven watchtower, blades and spells ready as forty orcs charge in. The stout warrior cleaves into them, slicing off four heads in two vicious cuts.

Our heroes stand atop a cliff of ice, a thousand foot drop behind them and twenty five wights in front, their eyes blazing blue and their black blades ready.

These are the tales of high adventure we know and love. We all remember Aragorn standing alone atop the ruined tower facing a horde of urukai in _Lord of the Rings_. We all remember John Wick facing off against a whole club of eastern European thugs. And we all remember the [seven samurai](https://slyflourish.com/seven_samurai_dnd.html) facing off against fifty town-ravaging bandits.

![](https://slyflourish.com/images/skeletal_hordes.jpg)

The mechanics of D&D combat generally presumes the characters will face somewhere between three and twelve bad guys in any given battle. This is why characters have a [huge advantage against a single opponent](https://slyflourish.com/improving_boss_fights.html).

Our stories need not be limited by these mechanics. We can, with a little work, run any number of monsters against the characters. Ten? Twenty? Two hundred? Ten thousand?

There are many imperfect ways to run huge hordes of monsters in D&D—situations in which the characters face twenty or more monsters in a single battle. They all require some level of abstraction from our standard combat rules. Some are simpler than others. Some use tables, others you can do in your head. You may have your own preference while other DMs have theirs.

In this article we focus on one particular method for running hordes. I selected this one for a few reasons:

-   You can do the math mostly in your head.
-   It doesn't take much more time than running smaller numbers of monsters.
-   It scales to any number of monsters we can imagine.
-   It still treats members of a horde as separate monsters when it matters to the players.
-   It focuses on the fiction of the situation instead of getting bogged down in mechanics.

## Summary Guidelines for Running Hordes

Here's a summary of my preferred techniques for running hordes. It breaks down into three large parts: tracking the damage done to the horde, tracking the horde's attacks and damage, and adjudicating areas of effect.

**Tracking Damage Done to the Horde**

-   Track damage inflicted to the horde instead of individual monsters in a single damage tally.
-   Write down the hit points of a single monster in the horde to keep track of it. Round it to the nearest 5 or 10 to make the math easier.
-   When the damage tally takes enough to kill one or more monsters in the horde, remove those monsters, reset the tally to zero, and carry over extra damage.

**Tracking Horde Attacks and Damage Output**

-   Determine how many monsters in the horde attack a given character based on the circumstances of the battle. When in doubt, divide attacks equally among those characters the horde can reasonably attack.
-   When the horde attacks, **assume one in four attacks succeed**. If the horde has advantage, assume half succeed. If they have disadvantage, assume they all fail. Adjust this up or down depending on circumstances. If someone casts _shield_ or has a crazy high AC, remove a couple of successful attacks.

**Adjudicating Areas of Effect**

When the horde is hit with an area of effect like _turn undead_, _hypnotic pattern_, or _fireball_, adjudicate the results with these guidelines:

-   Determine how many creatures are in the area of effect. Assume it's a lot of them.
-   Assume **one in four creatures in the horde succeed on their saving throws**. Adjust this up or down depending on the circumstances. For a truly heroic moment or to make your life easier, assume they all fail.
-   If the horde takes damage high enough to kill a single creature, remove all affected creatures. Extra damage doesn't carry over.
-   If monsters in the horde are incapacitated, separate them from the main horde and remove them from play.
-   Add up any remaining damage done to creatures who survive and add it to the current tally for the horde. If this kills more creatures, remove them, reset the damage to zero, and roll over remaining damage.

**Other Tips for Running Hordes**

-   Use evocative narration to describe the characters' heroic battle against huge hordes of enemies. Hordes are there to show off the might and heroism of the characters.
-   Use only one type of creature in the horde. Don't mix up multiple horde types in a single battle. Use the same stat block and create variance in your descriptions.
-   As desired, mix in normal monsters with your hordes. A horde of forty creatures might be led by four lieutenants and a boss. Run these extra monsters as you normally would.

The rest of this article dives deeper into each of these ideas.

## A Variety of Systems

This system for handling hordes is just one method of many. Other methods include:

-   The "Handling Mobs" section in chapter 8 of the  DMG [[#Handling Mobs]]
-   The "Running Large Numbers of Monsters" section of the _[Lazy DM's Workbook](https://slyflourish.com/lazydmsworkbook/index.html)_.
-   4e-Style "minion" rules in which each monster in a horde only has one hit point but a successful save never kills them.
-   The [[#Mob Damage Calculator]] (https://slyflourish.com/mob_calculator.html).
-   [[Syl Flourish Reskinning bigger monsters as a horde of smaller ones]](https://slyflourish.com/high_level_swarms.html).

It's possible you will prefer one of these other systems to the one proposed in this article. That's fine. What works well for you and your group is the one that matters. The end of this article describes the advantages and disadvantages of these alternate systems.

## The Basics of Running Hordes

When we're running large hordes of monsters in our D&D games, we generally skip the use of miniatures and we worry less about any individual creature in our battle.

We run these huge battles mostly in our descriptions augmented by some quick sketches of the situation. The players may want to find choke points where they can't be attacked by the whole horde all at once. We can use miniatures for the characters and then draw large blobs to represent the hordes and the groups they form up into. If the characters are defending a tower from a horde of orcs and there are three ways into the tower, we can represent the tower and place the characters' miniatures so that they can clearly see where the choke points are. We don't need forty orc miniatures, a big handdrawn blob with "orcs" in the center works just as well. People will get the idea.

Our goal in these battles is to **adjudicate the situation**. What makes sense given the current story and situation?

## Tracking Damage: Tallying Damage Against the Whole Horde

When we begin a battle against a horde, we write down the number of creatures in the horde and the hit points of one creature within the horde. Round their average hit points to the nearest 5 or 10 to make life easier.

When the characters attack the horde, they still attack versus the AC of a single monster in that horde. When they damage the monster, add the damage to the single damage tally for the whole horde. If the tally goes above the hit points of a single creature, we remove the last creature damaged from the horde, reset the tally, and roll over any remaining damage. This is similar to the "Cleaving through Creatures" description in chapter 9 of the _Dungeon Master's Guide_. A single powerful blow might kill multiple creatures which, of course, is awesome.

For example, a fighter faces off against a horde of skeletons and hits them with three attacks, inflicting 36 damage. We remove three of the skeletons (10 hp each) and add 6 damage to our tally. Next turn a rogue backstabs a skeleton for 19 damage. We add 19 to the 6 (25), remove two more skeletons and roll over 5 to the damage tally.

If a bunch of monsters in a horde are damaged with an area attack spell, we first figure out how many monsters in the horde it hits and then apply the damage to those who would be hit. If the damage is higher than the hit points of a single monster, we remove them all and don't worry about rolling over excess damage. If they don't take enough damage to kill them, we add it all up on the tally and see how many monsters it might kill.

For example, a wizard casts fireball on a horde of zombies and we adjudicate that it can hit sixteen zombies (20 hp each). The wizard rolls 27 damage for the fireball. Three quarters of the zombies fail their saving throw, taking 27 fire damage each, and are instantly killed. The remaining four take 13 damage each or 52 total added to the tally. This is enough to kill two more and leave 12 damage on the tally. Two zombies remain, one badly scorched.

This tally idea seems complicated but it scales well for any number of monsters. You can run a dozen orcs this way, or one hundred skeletons, or five hundred goblins and the same system applies.

**Track damage done to the whole group in a damage tally and remove monsters as the group takes enough damage to kill a single monster.**

## Adjudicating Which Characters Get Attacked

It's possible, given the size of the horde, to just use the damage tally idea above and still roll monster attacks normally. If you're running around twenty creatures with single attacks, rolling individual attacks isn't so bad. If you're running a LOT of monsters, though, you may want to abstract the attacks to speed up gameplay.

First, you need to decide who's getting attacked by the horde and how many monsters within the horde are attacking them. Start by looking at the situation. Does the horde have ranged attacks? Are any of the characters up front and likely to take on more than everyone else? Our base assumption should be that **the monsters attack the characters equally**. If there are fifty orcs and five characters, ten orcs will attack each character. If one character manages to hide from the orcs, the orcs divide their attacks among the rest. If a circumstance means that the monsters simply can't attack, for example if there's a choke point and they don't have ranged attacks, they miss out.

**Determine based on the circumstances how many within a horde attack each character. Begin by assuming they divide their attacks equally.**

## About One in Four Attacks Succeed

In any given match up between weak monsters and strong characters—the likely situation when a horde attacks the characters—we can assume that about one in four monsters in the horde will hit when they all attack.

This is a loose approximation and we can adjust it based on circumstances. Such circumstances might include:

-   The characters have extraordinarily high ACs, like the use of a _shield_ spell or some other big boost to AC.
-   A character has a particularly low AC and might get hit more often.

In these circumstances we can either choose to round up or down when determining how many creatures succeed or, if its a big enough bonus, we can change it from one in four succeeding to one in eight or one in ten if things are going against them or one in two if they have advantage.

Start with one in four and then slide the gauge up or down depending on the situation. This is a nearly math-less way of determining how many monsters succeed or fail that we can do in our heads without the use of a table or tool. Thus, [it's the lazy way](https://slyflourish.com/returnofthelazydm/index.html).

If the horde has advantage, such as those having _pack tactics_, we might increase this to half of them succeeding. Likewise, if they are at disadvantage, we might lower it to one in ten succeeding, or even less.

When the creatures in a horde have multiple attacks, we pool all of those attacks together to decide how many total attacks hit. If eight thugs attack a single character with their _multitattack_, we begin by assuming two of them hit with both attacks (one out of four of them) but remembering that the thugs have _pack tactics_, we might increase that to four successful thugs and eight total attacks hitting for 5 damage each (40 damage). Thugs make dangerous hordes.

**Assume one in four monsters succeed on their attacks and adjust accordingly.**

## Adjudicating Areas of Effect

When the characters face off against a large number of monsters, they're almost certainly going to fall back to area of effect spells like _fireball_, _cone of cold_, _shatter_, _turn undead_, or _hypnotic pattern_. Adjudicating areas of effect against large numbers of monsters takes a few steps but once these steps are wired in, it isn't too hard.

-   First, figure out how many creatures are in the area of effect based on the situation. Are the monsters all packed up together? Are they spread out? Consider the size of the area and how many you would think would be piled in there. Lean towards lots of monsters being within the area of effect. It's cooler that way.
-   Assume one in four monsters succeed on their saving throws and adjust to suit the situation. For a more heroic situation, assume they all fail the saving throw and describe the awesome results. Don't nitpick the details, round in favor of the characters and focus the description on their success.
-   If the damage of the area of effect inflicts enough to kill a single creature, those creatures die and are removed from the horde. If it's close (like a 14 point fireball against skeletons with 15 points), make your life easy and kill them anyway.
-   Add up the remaining damage that didn't kill the creatures and add it to your horde damage tally. This may kill additional creatures so remove them too.
-   If the effect includes a status effect of some sort; three out of four of the creatures will have failed and are under that status effect. You might remove them from play and describe their impotent attacks in the narrative instead of tracking things.

These steps might seem complicated but most of the time it will work out well. Areas of effect should be very useful against huge hordes of enemies.

**When hit with an area of effect, determine how many creatures are in the area, roll damage, remove those who die, carry over any remaining damage to the horde and remove additional dead creatures.**

Many areas of effect abilities, such as _turn undead_, don't inflict damage but inflict some other status effect. In this case, we can assume that one in four succeeds while the others fail. We can keep track of these incapacitated enemies separate from the rest of the horde or simply remove them from play. When a character wants to target one of the creatures who are under the status; like a skeleton restrained by an _Evard's black tentacles_ spell, they can simply state it and we adjust accordingly.

## Calculating Challenge Ratings

I've talked here at length about the [flaws of D&D's encounter building rules](https://slyflourish.com/5e_encounter_building.html) and [offered numerous solutions](https://slyflourish.com/the_lazy_encounter_benchmark.html). Many times when facing huge hordes of monsters, the encounter is very likely deadly. This goes up significantly if the challenge rating of the monsters in the horde are higher than CR 1/4 or 1/2.

You can still use my [simple encounter building](https://slyflourish.com/the_lazy_encounter_benchmark.html) guidelines to determine this however, and get an idea how many monsters in a horde are on that edge of deadly. Here's a summary of my simplified encounter building rules:

**An encounter is potentially deadly if the sum total of monster challenge ratings is greater than half of the sum total of character levels, or one quarter if the characters are below 5th level.**

Thus, if we have five 10th level characters, we know that more than 100 skeletons in a horde is potentially deadly. If we have five 7th level characters, more than 34 thugs is potentially deadly.

These battles against hordes can swing one way or another easily, though, given the sheer number of them and the potential to get wiped out with big areas of effect so, of course, your mileage will vary.

**Don't hang on too tight to encounter building rules when running hordes.**

## Other Guidelines for Running Hordes

That covers the basics of running monster hordes. Here are a few tips to make running huge battles easy and memorable.

**Go big with descriptions.** These battles are all about epic storytelling. Don't focus on the mechanics in your descriptions. Instead, focus on the story. Describe the screaming hordes of orcs charging the characters only to be blown away by a fireball. Describe the hordes of skeletons charging up the hill or the silent wights marching forward. Focus on the fiction first and last. Let the mechanics help shape the story.

**Use the same type of monster for the horde.** Don't try to run multiple monster types in a single horde. Trying to track two different hordes is really difficult and gods help you if those hordes get mix up together.

**Reflavor for variance.** If the story dictates that the horde has different kinds of creatures in them, use a single stat block and reflavor the creature in your descriptions. If the characters are getting attacked by both pirates and sea spawns; use a single stat block to represent them. In your description you describe some of them as more humanoid looking pirates and others as more twisted sea creatures. Yet, for you, the stat block is still the same. No one will be the wiser.

**Use three groups or fewer.** When you split up your hordes into separate horde groups, keep them around three or fewer. One is best and easiest to work with. More than three and life gets complicated.

**Mix hordes with normal creatures.** While running multiple types hordes can be difficult, a single horde can work well when mixed with normal single creatures. A horde of fifty orcs might be led by an orc war chief and four armored ogres. You can run the war chief and the ogres as individual creatures like normal and the horde using the guidelines above. It will make for a complicated fight but it isn't out of the question.

Now let's take a brief look at some alternate systems for running monster hordes.

## Alternate System: The Dungeon Master's Guide Mob Rules

Page 250 of the [[202202101110 5e DnD DMG Dungeon Masters Guide]] includes a brief section called "Handling Mobs" with instructions and a table to help adjudicate hits when lots of monsters are attacking a single character. The general idea is that, instead of rolling dice, you figure out how many monsters are _likely_ to hit given their attack bonus and the AC of their victim. We can use the same table in reverse to determine how many creatures make their save against a characters' spell or ability.

The guidelines in the DMG are solid. If you have the table on hand, it's a fine way to adjudicate how many monsters succeed in an attack. You can also reverse-engineer this table to also determine how many monsters would succeed on a saving throw.

Unfortunately, these guidelines don't tell us how to easily track hit points for a large number of monsters so we need some other system for tracking hit points. The horde damage tally can work well for this.

## Alternate System: The Lazy DM Workbook Table

Page 7 of the _[Lazy DM's Workbook](https://slyflourish.com/lazydmsworkbook/index.html)_ includes a table similar to the one in the _Dungeon Master's Guide_ and offers a way to track hit points by building a huge hit point pool for all of the monsters and then every time that pool takes damage equal to the hit points of a single monster, removing that monster. This latter part is actually difficult when used at the table and I now prefer the solution in this article. The table itself, however, continues to serve in the same way the one in the DMG serves.

## Alternate System: 4e-Style Minion Rules

If we want a simpler system for tracking damage done to monsters, we can steal the idea of "minions" from the 4th edition of D&D. In this system, every creature in the horde has only one hit point. If they take damage, they die. They take no damage if they succeed on a saving throw, however, so you can't just wipe them out with a single fireball unless they all fail their saving throw. Damage, in this case, does _not_ carry over.

This system works well by requiring no bookkeeping. Monsters are either alive or dead. They don't actually have hit points. If they are hit, they die. If they are missed, they survive. It's a deviation from the core rules but a clean system none the less.

## Alternate System: The Mob Damage Calculator

A while back I wrote a [mob damage calculator](https://slyflourish.com/mob_calculator.html) intended to help DMs determine how many monsters succeed on attacks or saving throws. You plug in the data and it spits out the results. This script works well enough but requiring a script to figure this out isn't ideal. Thus, I recommend easier systems for determining success. If you prefer this to other systems, go with the gods.

## Alternate System: Reskinning Bigger Monsters into Swarms

Likewise, I wrote another article on [reskinning big monsters into swarms](https://slyflourish.com/high_level_swarms.html). This system seems elegant but it fails as soon as the characters try to hit the "swarm" with an area of effect spell. A fireball should be very effective against a swarm yet does nothing special to a single big monster treated as a swarm. The same is true with spells like _hypnotic pattern_ or abilities like _turn undead_. Against a big monster swarm, its either all on or all off. That isn't ideal. Thus, I prefer systems that still treat monsters in a horde individually.

## Another Tool for Fantastic Stories

This article outlines a simple system for running large numbers of creatures against your characters. As [lazy dungeon masters](https://slyflourish.com/returnofthelazydm/index.html), we let the story take us where it will and use the tools we have on hand to make them as exciting and fantastic as possible. Now when our epic heroes are standing on a mountain of bones in the undead world of Thanatos surrounded by two hundred ghouls, you have the tools on hand to let the story flow into this epic situation.

## Related Articles