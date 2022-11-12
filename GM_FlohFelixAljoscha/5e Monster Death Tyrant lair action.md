A Death Tyrant’s Lair

A death tyrant’s lair is usually the same site it held as a beholder, but it contains more trappings of death and decay. A death tyrant encountered in its lair has a challenge rating of 15 (13,000 XP).
 

Lair Actions

When fighting inside its lair, a death tyrant can invoke the ambient magic to take lair actions. On initiative count 20 (losing initiative ties), the death tyrant can take one lair action to cause one of the following effects:

 An area that is a 50-foot cube within 120 feet of the tyrant is filled with spectral eyes and tentacles. To creatures other than the death tyrant, that area is lightly obscured and difficult terrain until initiative count 20 on the next round.
    Walls sprout spectral appendages until initiative count 20 on the round after next. Any creature, including one on the Ethereal Plane, that is hostile to the tyrant and starts its turn within 10 feet of a wall must succeed on a DC 17 Dexterity saving throw or be grappled. Escaping requires a successful DC 17 Strength (Athletics) or Dexterity (Acrobatics) check.
    A spectral eye opens in the air at a point within 50 feet of the tyrant. One random eye ray of the tyrant shoots from that eye, which is considered to be an ethereal source, at a target of the tyrant’s choice. The eye then closes and disappears.

The death tyrant can’t repeat an effect until all three have been used, and it can’t use the same effect on consecutive rounds.


```statblock
image: null
name: Death Tyrant
size: large
type: undead, monster manual
alignment: lawful evil
ac: 19
hp: 187
hit_dice: 25d10+50
speed: 0 ft., fly 20 ft. (hover)
stats:
  - 10
  - 14
  - 14
  - 19
  - 15
  - 19
saves:
  - strength: 5
  - constitution: 7
  - intelligence: 9
  - wisdom: 7
  - charisma: 9
skillsaves:
  - Perception: 12
damage_immunities: poison
condition_immunities: charmed, exhaustion, paralyzed, petrified, poisoned, prone
senses: darkvision 120 ft.
languages: Deep Speech, Undercommon
cr: "14"
traits:
  - name: Negative Energy Cone
    desc: The death tyrant's central eye emits an invisible, magical 150-foot cone
      of negative energy. At the start of each of its turns, the tyrant decides
      which way the cone faces and whether the cone is active. Any creature in
      that area can't regain hit points. Any humanoid that dies there becomes a
      zombie under the tyrant's command. The dead humanoid retains its place in
      the initiative order and animates at the start of its next turn, provided
      that its body hasn't been completely destroyed.
spells: []
actions:
  - name: Bite
    desc: "Melee Weapon Attack: +5 to hit, reach 5 ft., one target. Hit: 14 (4d6)
      piercing damage."
  - name: Eye Rays
    desc: "The death tyrant shoots three of the following magical eye rays at random
      (reroll duplicates), choosing one to three targets it can see within 120
      ft. of it: 1. Charm Ray. The targeted creature must succeed on a DC 17
      Wisdom saving throw or be charmed by the death tyrant for 1 hour, or until
      the death tyrant harms the creature. 2. Paralyzing Ray. The targeted
      creature must succeed on a DC 17 Constitution saving throw or be paralyzed
      for 1 minute. The target can repeat the saving throw at the end of each of
      its turns, ending the effect on itself on a success. 3. Fear Ray. The
      targeted creature must succeed on a DC 17 Wisdom saving throw or be
      frightened for 1 minute. The target can repeat the saving throw at the end
      of each of its turns, ending the effect on itself on a success. 4. Slowing
      Ray. The targeted creature must succeed on a DC 17 Dexterity saving throw.
      On a failed save, the target's speed is halved for 1 minute. In addition,
      the creature can't take reactions, and it can take either an action or a
      bonus action on its turn, not both. The creature can repeat the saving
      throw at the end of each of its turns, ending the effect on itself on a
      success. 5. Enervation Ray. The targeted creature must make a DC 17
      Constitution saving throw, taking 36 (8d8) necrotic damage on a failed
      save, or half as much damage on a successful one. 6. Telekinetic Ray. If
      the target is a creature, it must succeed on a DC 17 Strength saving throw
      or the death tyrant moves it up to 30 ft. in any direction. It is
      restrained by the ray's telekinetic grip until the start of the death
      tyrant's next turn or until the death tyrant is incapacitated. If the
      target is an object weighing 300 pounds or less that isn't being worn or
      carried, it is moved up to 30 ft. in any direction. The death tyrant can
      also exert fine control on objects with this ray, such as manipulating a
      simple tool or opening a door or a container. 7. Sleep Ray. The targeted
      creature must succeed on a DC 17 Wisdom saving throw or fall asleep and
      remain unconscious for 1 minute. The target awakens if it takes damage or
      another creature takes an action to wake it. This ray has no effect on
      constructs and undead. 8. Petrification Ray. The targeted creature must
      make a DC 17 Dexterity saving throw. On a failed save, the creature begins
      to turn to stone and is restrained. It must repeat the saving throw at the
      end of its next turn. On a success, the effect ends. On a failure, the
      creature is petrified until freed by the greater restoration spell or
      other magic. 9. Disintegration Ray. If the target is a creature, it must
      succeed on a DC 17 Dexterity saving throw or take 45 (10d8) force damage.
      If this damage reduces the creature to 0 hit points, its body becomes a
      pile of fine gray dust. If the target is a Large or smaller nonmagical
      object or creation of magical force, it is disintegrated without a saving
      throw. If the target is a Huge or larger object or creation of magical
      force, this ray disintegrates a 10-foot cube of it. 10. Death Ray. The
      targeted creature must succeed on a DC 17 Dexterity saving throw or take
      55 (10d10) necrotic damage. The target dies if the ray reduces it to 0 hit
      points."
legendary_actions:
  - name: Eye Ray
    desc: The death tyrant uses one random eye ray.
reactions: []
source: Monster Manual
```