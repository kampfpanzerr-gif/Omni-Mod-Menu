# Omni Mod Menu

An in-game mod menu for **Risk of Rain 2**. Press **Insert** in a run to open it.

Everything is in one window: character and item tools, spawning, teleports, an item X-ray, stat editing, music, on-screen counters, themes, hotkeys, and a global search that finds any of it by name. The interface comes in **12 languages**.

> Omni is a cheat-style menu. Use it in single-player or in lobbies where everyone agrees to it. Most of the "world" features only work for the **host**, and using them to spoil other people's games is on you.

## Features

**Player**
- God mode, fly (Space up / Ctrl down / Shift faster), noclip, infinite jumps, free purchases
- Aimbot with field of view, range, smoothing and a "visible targets only" option
- Infinite charges, set **separately** for primary, secondary, utility, special (ultimate) and equipment
- Move speed, attack speed, jump power, armor, crit chance and crit damage
- Gold, lunar coins, levels, full heal, clear inventory

**Items, equipment, characters**
- Every item and equipment with the game's own icons, colored by rarity and grouped by type, with search and filters
- Add or remove items in any amount
- Switch to any character in the middle of a run. Characters from a DLC you do not own (or that is off in the run) are grayed out and locked, because selecting them breaks the game

**Teleport**
- To any stage, to the teleporter (the boss portal), to other portals, to any object on the map, to an ally, or bring an ally to you

**Drones and spawning**
- Summon any drone, spawn any enemy or ally in any amount

**Scanner (X-ray / ESP)**
- See items through walls, including **what is inside chests and shops**, with icons and rarity colors and a rarity filter
- Highlight enemies and players with boxes, health bars and distance
- Optional snap lines, separately for enemies, players and items

**Players tab (host)**
- For every player in the world: god mode, heal, revive, kill, money, items, equipment, stat multipliers (including armor and crit), teleport to the player or bring them to you, and **kick**

**World**
- Charge the teleporter instantly, open all chests, kill all enemies or only bosses, next stage, disable enemy spawning, game speed

**Music**
- Pick any track from the game's own soundtrack with its length shown, reset to the stage default, and set the music volume

**Interface**
- Counters for **FPS** and **ping** (simple or detailed), shown even with the menu hidden. Color, outline, size and position are adjustable
- A list of your active features in a screen corner, optional "Hide HUD" for screenshots
- Color themes (including rainbow and gradients), custom colors and backgrounds, scale and opacity
- Rebindable hotkeys, a main and an extra key for each action, with a warning if the key is already used
- Global search over functions, items, equipment, characters, drones, enemies, stages and music

## Languages

English, Українська, Русский, Deutsch, Español, Français, Italiano, Português (BR), Türkçe, 日本語, 한국어, 简体中文.

The menu starts in the language of the game and remembers the language you pick. Item, character and stage names always follow the game's own language.

To add or fix a translation, edit the `.json` files in the `lang` folder next to the plugin. Each file is a flat `"English text": "translation"` list. Missing entries fall back to English.

## Installation

**Mod manager (recommended):** install with r2modman or Thunderstore Mod Manager. The required BepInEx is installed automatically.

**Manual:**
1. Install BepInExPack (`bbepis-BepInExPack`).
2. Copy the `OmniModMenu` folder into `Risk of Rain 2/BepInEx/plugins/`. It must contain `OmniModMenu.dll`, the `lang` folder and `music_durations.json`.
3. Start the game.

## Using it

- **Insert**: open or close the menu (rebindable in Settings).
- Drag the title bar to move the window, drag the bottom-right corner to resize it.
- While the cursor is over the menu, the menu is meant to stop the game from receiving your clicks and keys.
- Settings are saved to `BepInEx/config/user.omni.modmenu.cfg`.

## Notes and limitations

- This is a first release. It reads and changes the game's internals, so a game update can break individual features.
- Stats, spawning, teleporting, kicking and the "Players" tab work only for the host.
- Changing the music volume changes the game's own music volume setting.
- The song length in the music tab is the length of the song's main loop, read from the game's sound bank. Some utility tracks have no value.
- Not tested together with other mods that change the camera, input, or the same stats.

## Troubleshooting

- **The menu does not open:** make sure the game was started through the mod manager (or that `winhttp.dll` is in the game folder for a manual install) and check `BepInEx/LogOutput.log` for errors from `Omni Mod Menu`.
- **A key does not respond:** another action may use it. Rebind it in Settings, where conflicts are shown.
- **A feature does nothing:** many need a living character in a run, and some need to be the host.

## Credits and legal

Built on BepInEx and HarmonyX. Not affiliated with or endorsed by Gearbox Publishing or Hopoo Games. Risk of Rain 2 is a trademark of its owners.
