# What this patch changes

Everything below is compared with PlanetChili's V2.0 patch. Each release includes every change listed here, so always use the latest patch.

## Dice and combat rules
- **Fair dice:** the game's dice were not fair. When the random number was out of range, the game cut it down instead of rolling again, so the middle faces came up far more often. On a d20, rolls of 1–4 and 17–20 came up 3.1% of the time each and 5–16 came up 6.25% each, so a natural 20 was 3.1%, not 5%. On a d6, 3 and 4 were twice as likely as the other faces; d10, d12 and d100 were uneven too. Every face is now equally likely. This affects every roll: to-hit, damage, saving throws, Thief skills, encounters and treasure. Averages are unchanged; even fights barely change, but long shots and "sure things" do:

  | Per 100 attacks | Before | Now |
  |---|---|---|
  | Even fight (needs 12+ on the die) | ~44 hits | ~45 hits |
  | Natural 20s / natural 1s | ~3 / ~3 | ~5 / ~5 |
  | Long shot (needs 18+) | ~9 hits | ~15 hits |
  | Near-certain (needs 5+) | ~88 hits | ~80 hits |

- **Saving throws:** each class has its own saving throw table across the five D&D categories (death ray/poison, wands, paralysis/turn to stone, dragon breath, spells), using the Rules Cyclopedia tables. Monsters save as Fighters of their Hit Dice. Before, everyone used the Fighter's save against spells for everything. Dwarves and Halflings benefit the most.
  - Which save applies: spider and scorpion poison, Troglodyte stench, Spitting Cobra spit, Create Poison and Disintegrate use death ray/poison; Ghoul, Gelatinous Cube and Carrion Crawler touches and the Basilisk gaze use paralysis/turn to stone; Wand of Fear and Wand of Paralyzation use wands; everything else uses spells.
- **To-hit:** hit chances improve by +2 per step, as in BECMI and the original game: Fighters, Dwarves, Elves and Halflings every 3 levels, Clerics and Thieves every 4, Magic-Users every 5.
- **Initiative:** monsters had -2 on every initiative roll. They now roll a plain d6, as in D&D.
- **Minimum damage:** every hit does at least 1 damage. Penalties could make a hit do nothing, or even heal the target.
- **Special attacks** (paralysing touches, stings, gazes, energy drain) follow the same rules as normal attacks, including natural 20 always hits and natural 1 always misses.
- **Penalties work:** negative modifiers such as Stench were read as bonuses. They are now applied as penalties.
- **Bows and slings:** the +1 Bow and +1 Sling use DEX to hit like the plain ones; the +3 Mace and the Staff use STR.

## Characters
- **Energy drain** removes the right hit points at levels 10 and 11, and no longer leaves current HP above the maximum.
- **XP needed:** Thief level 4 is 4,800, Halfling level 8 is 120,000 and Magic-User level 14 is 1,050,000, as in D&D. The status screen shows the right Thief level 5 amount (9,600).
- Thieves no longer shrug off healing, potions and buffs from their friends 1/16th of the time.

## Spells and items
- **Staff of Striking** is a melee weapon as in D&D: it rolls to hit, a hit does 2d6, and it can only wear out on a hit. It used to always hit, like a spell.
- **Magic Missile** does the original game's damage: 1 missile, plus 2 more every 5 levels, each 1d6+1.
- **Remove Fear** works and the fear does not come back.
- **Wand of Fear** wears out like other wands.
- **Ring of Protection +1** gives 1 better AC and +1 saving throws instead of 1 better AC, +1 To hit, and +1 to Damage.
- **Staff** does 1d6 instead of 1d4, as the D&D rules and the hint book state.
- **Ring of Water Walking** works (it did nothing before). It is not yet placed anywhere in the game.
  - While anyone in the party has the ring in **Items Carried**, the whole party can walk on rivers, lakes and their sandy banks, while exploring and in combat. Swamps, lava, cliffs and walls are unchanged. Monsters still cannot enter water.
  - While standing **on water**, a character cannot use A or B (no weapons, spells, abilities or healing), the party cannot rest, and items cannot be dropped. Sandy banks count as land.
  - Shown in STATUS EFFECTS as WATER WALKING for the character carrying it.
- Unused items repaired for modders: the six special +1 swords, Wand of Paralyzation, Horn of Blasting.

## Monsters
- Damage matched to the official hint book for the Black Dragon, Red Dragon, Green Dragon, Lion, Cave Bear, Fire Elemental, Giant Crab and Allosaurus (on average 0.5 more damage).
- Gecko has 4 Hit Dice.
- Tiny Beastman does 1–7 instead of 0–7.
- Hellhounds are immune to fire.
- The Animated Corpse is undead, like the Zombie it is based on.

## Readied weapons (A and B)
- **Kept when you still carry a copy:** with a weapon readied on A or B, picking up a second copy and then selling, dropping or giving away either one cleared A/B, even though the character still carried the weapon. A/B is now cleared only when no copy is left.
- **Cancelling an action no longer corrupts A/B:** cancelling after Chili's automatic inventory opening could replace the B item with an unrelated item. The action is now restored correctly.

## Controls and convenience
- **Change Roster Order stays open** after each swap, so you can reorder the whole party in one visit. Press Start when done. The swap is also immediate: the cursors no longer blink for about 2 seconds.
- **6-button pad shortcuts on the map:** X opens Inventory and Y opens View Map, then return to the map, as if chosen from Camp. Y only opens a map you have (in dungeons, or once you own the area's map). Start still opens Camp. Set your emulator's or flash cart's pad to 6-button; on a 3-button pad nothing changes.

## Screens and information
- **OPTIONS > STATUS EFFECTS:** lists every active effect on the selected character, with remaining time and a description of what it does. C changes character.
- **Shop comparisons:** in weapon and armour shops, BUY shows your current A/B weapons against the highlighted one (hit chance against AC 0 and damage range), or your current and new AC for armour and shields, including active modifiers. C changes character. Nothing is equipped or changed until you buy.
- **Stench** is shown as a condition in the party status display.
- **Gauntlets of Ogre Power** show their own artwork on the ground and when picked up (they used another item's sprite).
- Fixed damaged walking frames after using OPTIONS > STATUS EFFECTS or a shop's BUY screen.

## Left out on purpose
A few of PlanetChili's V2.0 changes are balance choices rather than fixes, so this patch uses the BECMI values instead. They are kept for a separate, optional Balance patch, still in development.
- Chili's faster to-hit tables (later steps +3 instead of +2).
- Chili's to-hit swap that gave the Thief the Fighter's rate and the Elf the Cleric's rate.
- Chili's INT bonus to Magic Missile damage.
