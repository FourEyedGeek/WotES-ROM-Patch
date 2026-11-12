# Changelog

All changes are relative to PlanetChili's V2.0 patch.

## v0.51

### Combat
- **Initiative:** monsters had -2 on every initiative roll. They now roll a plain d6, as in D&D.
- **Minimum damage:** every hit does at least 1 damage. Penalties could make a hit do nothing, or even heal the target.
- **Special attacks** (paralysing touches, stings, gazes, energy drain) follow the same rules as normal attacks, including natural 20 always hits and natural 1 always misses.
- **Bows and slings:** The +1 Bow and +1 Sling now use DEX to hit like the plain ones; the +3 Mace and the Staff use STR again.

### Monsters
- Damage matched to the official hint book for the Black Dragon, Red Dragon, Green Dragon, Lion, Cave Bear, Fire Elemental, Giant Crab, and Allosaurus. This caused a 0.5 average increase in damage from them.
- Gecko has 4 Hit Dice.
- Tiny Beastman does 1-7, instead of 0-7.
- Hellhounds are immune to fire.
- The Animated Corpse is undead, like the Zombie it is based on.

### Characters
- **Energy drain** removes the right hit points at levels 10 and 11, and no longer leaves current HP above the maximum.
- **XP needed:** Thief level 4 is 4,800, Halfling level 8 is 120,000 and Magic-User level 14 is 1,050,000, as in D&D. The status screen shows the right Thief level 5 amount (9,600).

### Spells and items
- **Remove Fear** works and the fear does not come back.
- Thieves no longer shrug off healing, potions and buffs from their friends 1/16th of the time.
- **Wand of Fear** wears out like other wands.
- **Ring of Protection +1** gives AC and saving throws.
- **Staff** does 1d6 instead of 1d4, like D&D rules and handbook states.
- Unused items repaired for modders: the six special +1 swords, Wand of Paralyzation, Horn of Blasting.

### Screens
- Fixed damaged walking frames after using OPTIONS > STATUS EFFECTS or a shop's BUY screen.

## v0.40b – first public release

### Fixes
- **Combat cancel corrupting A/B:** cancelling an action after Chili's automatic inventory opening could replace the B item with an unrelated item. The action is now restored correctly.
- **Negative attack modifiers:** penalties such as Stench were read as unsigned values. They are now applied as penalties.
- **Gauntlets of Ogre Power graphics:** the gauntlets used another item's sprite on the ground and when picked up. They now show their own artwork.
- **Stench:** now shown as a condition in the party status display.
- **Ring of Water Walking:** this unused item did nothing. It now works (see below). The ring is not yet placed anywhere in the game.

### Added
- **OPTIONS > STATUS EFFECTS:** lists every active effect on the selected character, with remaining time and a description of what it does. C changes character.
- **Shop comparisons:** in weapon and armour shops, BUY shows your current A/B weapons against the highlighted one (hit chance against AC 0 and damage range), or your current and new AC for armour and shields, including active modifiers. C changes character. Nothing is equipped or changed until you buy.

### Ring of Water Walking
- While anyone in the party has the ring in **Items Carried**, the whole party can walk on rivers, lakes and their sandy banks, while exploring and in combat. Swamps, lava, cliffs and walls are unchanged. Monsters still cannot enter water.
- While standing **on water**, a character cannot use A or B (no weapons, spells, abilities or healing), the party cannot rest, and items cannot be dropped. Sandy banks count as land.
- Shown in STATUS EFFECTS as WATER WALKING for the character carrying it.
