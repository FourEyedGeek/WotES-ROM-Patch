# Changelog

All changes are relative to PlanetChili's V2.0 patch.

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
