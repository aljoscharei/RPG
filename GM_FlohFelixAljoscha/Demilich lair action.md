[[201508040820.2 00551 Neuro Locked-in]]
 [[lich lair actions]] mit Locked-in Syndrom bei pontiner myelinolyse
https://www.dndbeyond.com/monsters/demilich

A Demilich’s Lair

A demilich hides its earthly remains and treasures in a labyrinthine tomb guarded by monsters and traps. At the heart of this labyrinth rests the demilich’s skull and the dust from its other bones.

In its crypt, a demilich has access to lair actions and additional uses for its legendary actions. Its whole lair also has unique traits. A demilich in its lair has a challenge rating of 20 (24,500 XP).
 

Lair Actions

On initiative count 20 (losing initiative ties), the demilich rolls a d20. On a result of 11 or higher, the demilich takes a lair action to cause one of the following effects. It can’t use the same effect two rounds in a row.

    The tomb trembles violently for a moment. Each creature on the floor of the tomb must succeed on a DC 19 Dexterity saving throw or be knocked prone.
    The demilich targets one creature it can see within 60 feet of it. An antimagic field fills the space of the target, moving with it until initiative count 20 on the next round.
    The demilich targets any number of creatures it can see within 30 feet of it. No target can regain hit points until initiative count 20 on the next round.

Lair Traits

A demilich’s tomb might have any or all of the following effects in place:

The first time a non-evil creature enters the tomb’s area, the creature takes 16 (3d10) necrotic damage.
    Monsters in the tomb have advantage on saving throws against being charmed or frightened, and against features that turn undead.
    The tomb is warded against the magical travel of creatures the demilich hasn’t authorized. Such creatures can’t teleport into or out of the tomb’s area or use planar travel to enter or leave it. Effects that allow teleportation or planar travel work within the tomb as long as they aren’t used to leave or enter the tomb’s area.

If the demilich is destroyed, these effects fade over the course of 10 days.

```statblock
image: null
name: Demilich
size: tiny
type: undead, monster manual
alignment: neutral evil
ac: 20
hp: 80
hit_dice: 20d4
speed: 0 ft., fly 30 ft. (hover)
stats:
  - 1
  - 20
  - 10
  - 20
  - 17
  - 20
saves:
  - constitution: 6
  - intelligence: 11
  - wisdom: 9
  - charisma: 11
skillsaves: []
damage_resistances: bludgeoning, piercing, and slashing from magic weapons
damage_immunities: necrotic, poison, psychic, bludgeoning, piercing, and
  slashing from nonmagical weapons
condition_immunities: charmed, deafened, exhaustion, frightened, paralyzed,
  petrified, poisoned, prone, stunned
senses: truesight 120 ft.
cr: "18"
traits:
  - name: Avoidance
    desc: If the demilich is subjected to an effect that allows it to make a saving
      throw to take only half damage, it instead takes no damage if it succeeds
      on the saving throw, and only half damage if it fails.
  - name: Legendary Resistance (3/Day)
    desc: If the demilich fails a saving throw, it can choose to succeed instead.
  - name: Turn Immunity
    desc: The demilich is immune to effects that turn undead.
spells: []
actions:
  - name: Howl (Recharge 5-6)
    desc: The demilich emits a bloodcurdling howl. Each creature within 30 feet of
      the demilich that can hear the howl must succeed on a DC 15 Constitution
      saving throw or drop to 0 hit points. On a successful save, the creature
      is frightened until the end of its next turn.
  - name: Life Drain
    desc: The demilich targets up to three creatures that it can see within 10 feet
      of it. Each target must succeed on a DC 19 Constitution saving throw or
      take 21 (6d6) necrotic damage, and the demilich regains hit points equal
      to the total damage dealt to all targets.
legendary_actions:
  - name: Flight
    desc: The demilich flies up to half its flying speed.
  - name: Cloud of Dust
    desc: The demilich magically swirls its dusty remains. Each creature within 10
      feet of the demilich, including around a corner, must succeed on a DC 15
      Constitution saving throw or be blinded until the end of the demilich's
      next turn. A creature that succeeds on the saving throw is immune to this
      effect until the end of the demilich's next turn.
  - name: Energy Drain (Costs 2 Actions)
    desc: Each creature with in 30 feet of the demilich must make a DC 15
      Constitution saving throw. On a failed save, the creature's hit point
      maximum is magically reduced by 10 (3d6). If a creature's hit point
      maximum is reduced to 0 by this effect, the creature dies. A creature's
      hit point maximum can be restored with the greater restoration spell or
      similar magic.
  - name: Vile Curse (Costs 3 Actions)
    desc: The demilich targets one creature it can see within 30 feet of it. The
      target must succeed on a DC 15 Wisdom saving throw or be magically cursed.
      Until the curse ends, the target has disadvantage on attack rolls and
      saving throws. The target can repeat the saving throw at the end of each
      of its turns, ending the curse on a success.
reactions: []
source: Monster Manual
```