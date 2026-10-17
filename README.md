# GudaPlates

A customizable nameplate addon for World of Warcraft 1.12.1 (Vanilla) and Turtle WoW.

## Features

- **Debuff Tracking** - Shows debuffs on enemy nameplates with countdown timers
- **Rank-Aware Durations** - Correctly tracks debuff durations based on spell rank
- **Cast Bars** - Displays enemy cast bars on nameplates (requires SuperWoW)
- **Threat Indication** - Visual threat indicators for tanks
- **Health & Level Display** - Clean health bars with level and classification icons
- **Raid Icons** - Shows raid target icons on nameplates
- **Target Highlight** - Highlights your current target's nameplate
- **Hide Friendly Nameplates** - Hides friendly nameplates and makes them unclickable (on by default)
- **Hide Neutral Nameplates** - Hides neutral nameplates until they become your target or enter combat (on by default)

## Friendly and Neutral Nameplates

Both options are on the General tab of `/gp config`, in the third row under Nameplate Settings. Uncheck either one to get the normal behavior back.

GudaPlates turns off pfUI's and ShaguTweaks' nameplate modules while it's loaded, so their hide settings won't apply. Use these options instead.

**Hide Friendly** removes the whole nameplate, health bar included. To still see names and guild tags over friendly players and NPCs, turn on the player name, guild name, and NPC name options in the game's Interface Options.

**Hide Neutral** keeps neutral mobs out of the way until they matter. A neutral nameplate shows up again as soon as you target it or it enters combat, so a mob you pull never vanishes. With SuperWoW this check is exact. Without it, GudaPlates uses the aggro glow to tell when a neutral mob is in combat.

## Threat Colors

Defaults (changeable on the Colors tab, and restored by Reset Defaults):

| Role | State | Color |
|------|-------|-------|
| DPS/Healer | Mob attacking you (bad) | Red |
| DPS/Healer | High threat (warning) | Orange |
| DPS/Healer | Tank has it (good) | Green |
| Tank | You have aggro (good) | Green |
| Tank | Another tank has it | Light blue |
| Tank | Losing aggro (warning) | Orange |
| Tank | No aggro (bad) | Red |

## Requirements

- World of Warcraft (Vanilla)
- **SuperWoW is highly recommended** for full functionality

## SuperWoW Support

GudaPlates works best with [SuperWoW](https://github.com/balakethelock/SuperWoW) installed. SuperWoW provides:

- **GUID-based tracking** - Accurate debuff tracking per mob, even with same-named enemies
- **Cast bar detection** - See enemy spell casts on nameplates
- **Enhanced nameplate matching** - Reliable nameplate-to-unit association

Without SuperWoW, GudaPlates will fall back to name-based tracking which may be less accurate with multiple enemies of the same name.

## Installation

1. Download the ZIP from GitHub (Code → Download ZIP)
2. Extract the ZIP file
3. Rename the extracted folder from `GudaPlates-main` to `GudaPlates`
4. Move the `GudaPlates` folder to your `Interface\AddOns\` directory
5. Final path should be: `Interface\AddOns\GudaPlates\`
6. Restart WoW or `/reload` if already in-game

## Slash Commands

- `/gp` or `/gudaplates` - Show available commands
- `/gp role tank` - Set role to tank (shows threat loss indicators)
- `/gp role dps` - Set role to DPS/healer (shows threat gain indicators)
- `/gp overlap` - Toggle nameplate overlap mode
- `/gp timers` - Toggle debuff countdown timers

## Debuff Duration Database

GudaPlates includes a comprehensive spell database with correct durations for all ranks of:

- Warrior debuffs (Rend, Hamstring, Thunder Clap, etc.)
- Rogue debuffs (Rupture, Garrote, Kidney Shot, etc.)
- Mage debuffs (Frostbolt, Polymorph, etc.)
- Warlock debuffs (Corruption, Curse of Agony, etc.)
- Priest debuffs (Shadow Word: Pain, etc.)
- Druid debuffs (Moonfire, Rake, etc.)
- Hunter debuffs (Serpent Sting, etc.)
- And many more...

## Credits

Inspired by ShaguPlates and other classic nameplate addons.

## License

MIT License - Feel free to modify and distribute.
