---
abilitymodifiers: "+2 Dex, +2 Cha, –2 Wis"
blurb:
cssclasses: 
date created: Tuesday, August 22nd 2023, 4:01:13 pm
date modified: Wednesday, August 21st 2024, 7:56:16 pm
hitpoints: "4"
size: "medium"
sizeandtype: "Ifrits are Medium outsiders with the native subtype."
tags: []
type: "outsider (native)"
---

>[!infobox|right wsmed]
>`= choice(this.blurb, "![[" + this.blurb + "]]", "")`
> # `= this.file.name`
>
> |stats|
> |----|----|
> |hp|`= this.hitpoints`|
> |mods|`= this.abilitymodifiers`|
> |size|`= this.size`|
> |type|`= this.type`|
>
>
> |vitals|
> |----|----|
> |Average Height| `= this.height`|
> |Average Weight| `= this.weight`| 
> |Age of Maturity| `= this.maturity` |
> |Maximum Age| `= this.age`|
>
>`$= dv.page(dv.current().file.name).file.name + "-Card-Stats.jpg" ? dv.fileLink(dv.current().file.name + "-Card-Stats.jpg", true) : ""`
>
>`$= dv.page(dv.current().file.name).file.name + "-Card-Portrait.jpg" ? dv.fileLink(dv.current().file.name + "-Card-Portrait.jpg", true) : ""`
>
# Ifrit

[[Species_Ifrit.jpeg|Zeigen!]]
**Source**:: _Starfinder Fire Starters pg. 60_
Ifrits are the descendants of mortal species and creatures from the Plane of Fire, usually efreet. These native outsiders are fiercely independent and many see even their friends as tools to be used.

**Ability Modifiers** +2 Dex, +2 Cha, –2 Wis
**Hit Points** 4

## Size and Type

Ifrits are Medium outsiders with the native subtype.

## Darkvision

Ifrits have darkvision with a range of 60 feet.

## Fire Affinity

Ifrits have an instinctive affinity for fire, subtly bending it to their will. Once per day, an ifrit making an attack that deals fire damage can roll a single attack roll twice and use the higher result.

## Fire Resistance

The supernatural fire in ifrit blood grants them resistance 5 to fire.

## Spell-like Ability

Once per day, an ifrit can cast overheat as a spell-like ability. At 8th level, he can use this ability one additional time per day, and he gains a third use per day at 16th level. His caster level equals his level, and the save DC is equal to 11 +his Charisma modifier.

# Alternate Racial Traits

**Source**:: _Starfinder The Perfect Storm pg. 51_
The following are alternate racial traits for planar scions.

## Hot Fusion

**Source**:: _Starfinder The Perfect Storm pg. 53_
Sun-born ifrits sometimes inherit their stellar progenitor’s nuclear nature. An ifrit of 5th level or higher with this trait can cast irradiate once per day. At 12th level, they can use this ability one additional time per day. Their caster level equals their level, and the save DC is equal to 13 +their Charisma modifier.
This replaces an ifrit’s spell-like ability.

## Warp Fusion

**Source**:: _Starfinder The Perfect Storm pg. 53_
When a planar scion with this trait makes an attack or casts a spell that would deal acid, cold, electricity, fire, or sonic damage, they can instead choose to match half of that damage to the element of their heritage (fire for ifrits, acid for oreads, electricity for sylphs, or cold for undines).
This replaces each planar scion’s elemental affinity.
