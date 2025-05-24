Oblivion(Remastered) Vampirism System Re-Imagined

## Glossary
- CS: Construction Set
- Power: Spell that can be cast once a day
- PC: Player Character

## Mechanic Details

- Each feeding from **'Stage 4' vampirism back to 'Stage 1'** increments `vampirelevel` by 1
- A total of **20 levels**
- Each Level **improves**, for some **maintains**, Attributes and Skills that Vampirism already amplifies
- Adds new skills and attributes per stage
```
    - Agility Buff at Vampirism       25->100 = 5->20
    - Personality Buff at Vampirism   25->100 = 15->(-8)
    - Intelligence Buff at Vampirsim  25->100 = 15->0
```


## Spell -> Power

| CS-Power Name | In-Game Name | Effect | Available at Level | Available at Vampirism Stage |
| :---: | :---: | :---: | :---: | :---: |
| Vampire50AbsorptionLevel20 | Vampiric Absorption | Absorb Health 150pts, Absorb Fatigue 150pts | Level 20 | 50 |
| Vampire75AbsorptionLevel20 | Vampiric Absorption | Absorb Health 200pts, Absorb Fatigue 200pts | Level 20 | 75 |
| Vampire100AbsorptionLevel20 | Vampiric Absorption | Absorb Health 250pts, Absorb Fatigue 250pts | Level 20 | 100 |
| VampireTransparencyLevel10 | Subtle Persence | Chameleon 65%, Speed 35pts, Sneak 15pts | Level 8 | 50,75,100 |
| VampMetabolicAcceleratorSpell | Undead Metabolic Acceleration | Allows PC to immediately get to stage 4 Vampirism | Level 10 | 25,50,75,100 |

## Vampirism25-100 (An additional mechanic)

* **\[25-100]:**

  * `Resist Frost` = Magnitude: 10–40 *(Increasing with progressing stages; balancing out Weakness to fire)*

* **\[100]:**

  * `Absorb Spell` = Magnitude: 10 *(Insatiable and desperate hunger reflecting in one's being)*


## Vampirism25-100Att (An additional mechanic)

* **\[25-100]:**

  * `Intelligence` = Magnitude: 15–0 *(Decreasing with progressing stages)*
  * `Agility` = Magnitude: 5–20 *(Increasing with progressing stages)*
  * `Personality` = Magnitude: 15–8–0 *(Vamp25–Vamp75)*

* **\[100]:**

  * `Drain Personality` = Magnitude: 8


## Vampirism25-100Skill (An additional mechanic)

* **\[25-100]:**

  * `Mercantile` = Magnitude: 15–0 *(Decreasing with progressing stages)*
  * `Speechcraft` = Magnitude: 15–0 *(Decreasing with progressing stages)*
  * `Waterbreathing` *(Available at all stages)*


## VampirismExtraSunDamage\[DMGVALUE] *(From Lvl 10 to 20)*

* `Sun Damage` = Magnitude: 3–15 *(in increments of 3)*


## VampirismExtraWR\[1-10] *(Add at every level, but increase at every even level)*

* `Resist Normal Weapons` = Magnitude: 1–10


## VampirismExtraAttLevel\[2-20] *(Add at every level, but increase at every even level)*

* `Fortify Strength` = Magnitude: 1–12
* `Fortify Willpower` = Magnitude: 1–10
* `Fortify Speed` = Magnitude: 1–9
* `Fortify Agility` = Magnitude: 1–12


## VampirismExtraSkillsLevel\[1-19] *(Add at every level, but increase at every odd level)*

* `Fortify Acrobatics` = Magnitude: 1–15
* `Fortify Athletics` = Magnitude: 1–15
* `Fortify Destruction` = Magnitude: 1–12
* `Fortify Hand-to-Hand` = Magnitude: 1–15
* `Fortify Illusion` = Magnitude: 1–13
* `Fortify Mysticism` = Magnitude: 1–12
* `Fortify Sneak` = Magnitude: 1–13


# Ranks

* **Fledgling Vampire (1–8)**
* **Callous Vampire (9–15)**
* **Harrowing Vampire (16–19)**
* **Master Vampire (20)**


## Fledgling Vampire (1–8)

* `VampirismExtraAttLevel`: 2, 4, 6, 8
* `VampirismExtraSkillsLevel`: 1, 3, 5, 7
* `VampirismExtraWR`: 1, 2, 3


## Callous Vampire (9–15)

* `VampirismExtraAttLevel`: 10, 12, 14
* `VampirismExtraSkillsLevel`: 9, 11, 13
* `VampirismExtraWR`: 4, 5, 6
* `VampirismExtraSunDamage`:

  * Vamp75 = 3, 6
  * Vamp100 = 9


## Harrowing Vampire (16–19)

* `VampirismExtraAttLevel`: 16, 18
* `VampirismExtraSkillsLevel`: 15, 17
* `VampirismExtraWR`: 7, 8, 9
* `VampirismExtraSunDamage`:

  * Vamp75 = 9
  * Vamp100 = 12


## Master Vampire (20)

* `VampirismExtraAttLevel`: 20
* `VampirismExtraSkillsLevel`: 19
* `VampirismExtraWR`: 10
* `VampirismExtraSunDamage`:

  * Vamp75 = 12
  * Vamp100 = 15


## New Globals

* `LastFedVampHour` (0–23)
* `LastFedVampDay` *(Simple check, all we care about is that it's not the same day as before)*
* `VampStageUpdate`

  * 0 = not time for Vampire Stage update
  * 1 = time for Vampire Stage update
* `VampMetabolicAcceleratorCasted`

  * 0 = not casted
  * 1 = casted


## TODO

* Write out Prompts for Each Milestone level-up
* Add new Dreams
* Metabolic Acceleration: find a way to make it sound more vampiric or something
  * *Undead Metabolic Acceleration?*
* Fix spelling errors: `"Vampiric Absor*b*tion"`
