Oblivion(Remastered) Vampirism System Re-Imagined

## Glossary
- CS: Construction Set
- Power: Spell that can be cast once a day
- PC: Player Character

## Mechanic Overview 

\~ Each feeding from **'Stage 4'** vampirism back to **'Stage 1'** increments **`VampireLevel`** by 1   

\~ A total of **20 levels**   

\~ Each Level **improves**, for some **maintains**, Attributes and Skills that Vampirism already amplifies   

\~ Adds new skills, attributes, and effects to baseline Vampirism stages


## Spell -> Power

| CS-Power Name | In-Game Name | Effect | Available at Level | Available at Vampirism Stage |
| :---: | :---: | :---: | :---: | :---: |
| Vampire50AbsorptionLevel20 | Vampiric Absorption | Absorb Health 150pts, Absorb Fatigue 150pts | Level 20 | 50 |
| Vampire75AbsorptionLevel20 | Vampiric Absorption | Absorb Health 200pts, Absorb Fatigue 200pts | Level 20 | 75 |
| Vampire100AbsorptionLevel20 | Vampiric Absorption | Absorb Health 250pts, Absorb Fatigue 250pts | Level 20 | 100 |
| VampireTransparencyLevel10 | Subtle Persence | Chameleon 65%, Speed 35pts, Sneak 15pts | Level 8 | 50,75,100 |
| VampMetabolicAcceleratorSpell | Undead Metabolic Acceleration | Allows PC to immediately get to stage 4 Vampirism | Level 10 | 25,50,75,100 |

## Changes to CS Properties Vampirism25-100

| Effects | Vampirism 25 | Vampirism 50 | Vampirism 75 | Vampirism 100 | Reasoning |
| :---: | :---: | :---: | :---: | :---: | :--- |
| Resist Frost | 10 | 20 | 30 | 40 | To balance out weakness to fire, but not 1-to-1. Frost resistance is 10pts less than Fire Weakness |
Absorb Spell | -/- | -/- | -/- | 10 | "Seemingly insatiable and desperate hunger reflecting in one's being". Or in other words - just makes stage 4 vampirism a bit more interesting. |


## Vampirism 25-100 Attribute changes

| Attribute | Vampirism 25 | Vampirism 50 | Vampirism 75 | Vampirism 100 | Reasoning |
| :---: | :---: | :---: | :---: | :---: | :--- |
| Intelligence | 15 | 10 | 5 | 0 | Cyrodiil Vampires are different to that of, say, Vampires of Skyrim. Their innate advantages primarily revolve around social integration and collusion. Hence, it made sense to me that attributes like "Intelligence" and "Personality" would get a buff when vampire is fully fed, and, conversely, degrade as Cyrodiil Vampire progresses through stages of hunger. |
| Agility | 5 | 10 | 15 | 20 | As Cyrodiil Vampire becomes hungrier, I think they become more primal. It made sense for "Agility" to get a buff aslo, not just "Strength". |
| Personality | 15 | 8 | 0 | -8 | As Vampire becomes primal, their Personality, in my opinion, shouldn't just return to baseline but get drained. |


## Vampirism 25-100 Skill changes

| Skill | Vampirism 25 | Vampirism 50 | Vampirism 75 | Vampirism 100 | Reasoning |
| :---: | :---: | :---: | :---: | :---: | :--- |
| Mercantile | 15 | 10 | 5 | 0 | As mentioned previously, Cyrodiil Vampire's primary innate advtange is social. It made sense to me that "Mercantile" skill should go up at fully-fed stage and decrease back to baseline at most primal stage. |
| Speechcraft | 15 | 10 | 5 | 0 | Same reasoning as for "Mercantile". |
| Waterbreathing | Available | Available | Available | Available| Cyrodiil Vampires, and Vampires in general TES lore, are considered undead. It made sense to me that breathing is of little concern to the undead. |

# Level Up Mechanics

## Level-Up Mechanic: Additional Sun Damage 

CS Spell Name - `VampirismExtraSunDamage[DMGVALUE]` *(From Lvl 10 to 20)*


| Vampire Rank | Extra Sun Damage at Vampirism 25 | Extra Sun Damage at Vampirism 50 | Extra Sun Damage at Vampirism 75 | Extra Sun Damage at Vampirism 100 |
| :---: | :---: | :---: | :---: | :---: |
| Fledgling Vampire | 0 | 0 | 0 | 0 |
| Callous Vampire | 0 | 0 | Vamp Level 9-12 = 3; Vamp Level 13-15 = 6 | Vamp Level 9-15 = 9 |
| Harrowing Vampire | 0 | 0 | 9 | 12 |
| Master Vampire | 0 | 0 | 12 | 15 |

It made sense to me that as Vampire progresses and becomes *more* of a Vampire, they'd get more Sun-Damage. Keeps things interesting.

## Level-Up Mechanic: Additional Normal Weapons Resistance
CS Spell Name - `VampirismExtraWR[1-10]`

Vampire Character would gain +1 `Resistance to Normal Weapons` every even level until level 20.

## Level-Up Mechanic: Attributes
CS Spell Name - `VampirismExtraAttLevel[2-20]` 
> *Increments to various degrees at every even level*

* `Fortify Strength` = Magnitude: 1–12
* `Fortify Willpower` = Magnitude: 1–10
* `Fortify Speed` = Magnitude: 1–9
* `Fortify Agility` = Magnitude: 1–12


## Level-Up Mechanic: Skills 
CS Spell Name - `VampirismExtraSkillsLevel[1-19]` 
>*Increments to various degrees at every odd level*

* `Fortify Acrobatics` = Magnitude: 1–15
* `Fortify Athletics` = Magnitude: 1–15
* `Fortify Destruction` = Magnitude: 1–12
* `Fortify Hand-to-Hand` = Magnitude: 1–15
* `Fortify Illusion` = Magnitude: 1–13
* `Fortify Mysticism` = Magnitude: 1–12
* `Fortify Sneak` = Magnitude: 1–13


# Vampire Ranks

* **Fledgling Vampire:** Level 1–8
* **Callous Vampire:** Level 9–15
* **Harrowing Vampire:** Level 16–19
* **Master Vampire:** Level 20


## Fledgling Vampire (1–8)

* `VampirismExtraAttLevel`[2, 4, 6, 8]
* `VampirismExtraSkillsLevel`[1, 3, 5, 7]
* `VampirismExtraWR`[1, 2, 3]


## Callous Vampire (9–15)

* `VampirismExtraAttLevel`[10, 12, 14]
* `VampirismExtraSkillsLevel`[9, 11, 13]
* `VampirismExtraWR`[4, 5, 6]
* `VampirismExtraSunDamage`:
  * Vamp75 = 3, 6
  * Vamp100 = 9


## Harrowing Vampire (16–19)

* `VampirismExtraAttLevel`[16, 18]
* `VampirismExtraSkillsLevel`[15, 17]
* `VampirismExtraWR`[7, 8, 9]
* `VampirismExtraSunDamage`:
  * Vamp75 = 9
  * Vamp100 = 12


## Master Vampire (20)

* `VampirismExtraAttLevel`[20]
* `VampirismExtraSkillsLevel`[19]
* `VampirismExtraWR`[10]
* `VampirismExtraSunDamage`:
  * Vamp75 = 12
  * Vamp100 = 15


## Globals

| CS Global Name | Data-Type | Range |
| :---: | :---: | :---: |
| `VampLevel` | Short | 0-20 |
| `LastFedVampHour` | Float | 0.000 - 23.999 |
| `LastFedVampDay` | Short | 0 - 31 |
| `VampStageUpdate` | Short | 0 - 1 |
| `VampMetabolicAcceleratorCasted` | Short | 0 - 1 |

## Level-Up Messages
<details>

<summary>**(WARNING: SPOILERS)**</summary>

if ( VampireLevel == 1 )
  "You can feel yourself change.. As a result of enduring starvation, you grew stronger. You are now Fledgling Vampire."

elseif ( VampireLevel == 2 )
  "Your power grows.."

elseif ( VampireLevel == 3 )
  "You can feel yourself growing stronger..",

elseif ( VampireLevel == 4 )
  "With each drink, you get stronger.." 

elseif ( VampireLevel == 5 )
  "You can feel yourself developing into something more.." 

elseif ( VampireLevel == 6 )
  "Greater power is coursing through you now.." 

elseif ( VampireLevel == 7 )
  "Something greater faintly stirs in you.." 

elseif ( VampireLevel == 8 )
  "Violation of others in their most vulnerable allowed you to ascend further. You are now Callous Vampire."

elseif ( VampireLevel == 9 )
  "Hunger is satiatied, but not your ambition.." 

elseif ( VampireLevel == 10 )
  "Blood of another flows into you, nourishing your growth.."

elseif ( VampireLevel == 11 )
  "Faster, Stronger, More.."

elseif ( VampireLevel == 12 )
  "You can feel blood of another pouring through to your viscera, feeding your strength.."

elseif ( VampireLevel == 13 )
  "Sweet flavours of blood are melting all over your tongue, coating your mouth, filling you with strength.."

elseif ( VampireLevel == 14 )
  "A step closer to fulfilling your desire for more power.."

elseif ( VampireLevel == 15 )
  "You have become intimately familiar with power that comes from your condition. Blood of your victims nourished you and crystallized lessons you had learned in battle; However, there's more to become. You are now Harrowing Vampire."

elseif ( VampireLevel == 16 )
  "Blood fuels your change.."

elseif ( VampireLevel == 17 )
  "Stolen essense of another fulfills you.."

elseif ( VampireLevel == 18 )
  "Starvation, hunt, and subsequent success.."

elseif ( VampireLevel == 19 )
  "It's within your reach.."

elseif ( VampireLevel == 20 )
  "Vampirism is instinctive to you, it's as if you were born as such. Being anything else is a vague, distant sensation now. You've attained mastery over your condition. Many have been slain by your hands and fangs, and you briefly ponder your entire journey on the way here. However, blood-stained sweet memories are interrupted by a subtle growing sensation.. of hunger. Hunger as undying as you. You are now Master Vampire."

</details>


## TODO

* Add new Dreams
* Fix spelling errors: `"Vampiric Absor*b*tion"`
