# Sephiria QoL — Changelog

## 1.46.5

- Fixed the new-version prompt closing right away when entering the game, so it never showed up.

## 1.46.4

- The restart notice after an update now mentions that the new version takes effect once you enter the game from the title screen.

## 1.46.3

- Fixed the previous version's file being left behind in the mod folder after an update.

## 1.46.2

- Reworded the update prompt and its buttons: [Update now / Remind me later / Skip this update]
- Choosing "Update now" restarts the game automatically once the download finishes.
- The game is not restarted when you update mid-run with `/qol update`.
- Added [Open changelog] to the top row of the QoL settings window.

## 1.46.1

- The update prompt now appears as soon as the game starts, instead of after 20 seconds.
- It waits while the game's own startup dialogs are open (photosensitivity, privacy, language, cloud saves).

## 1.46.0

- The mod tells you in game when a new version is available and can download it for you.
- What you download takes effect the next time you start the game.
- The default is "ask, then install". You can turn it off or switch to "install without asking" under [Check for updates].
- Type `/qol update` in chat to check manually.

## 1.45.3

- Odner explosion range display is now a full-QoL setting, chosen by the host before a run and locked during it.
- Host and guests all need 1.45.3 or later to follow the same rules.
- Warning colors remain a personal setting.

## 1.45.2

- Removed the pass that re-checked every pending reward on each level-up and floor change for journal bans.

## 1.45.1

- Odner warnings now follow each bomb's actual position, including sliding after it lands.

## 1.45.0

- Fixed `/gd` and `/givedice` being blocked when dice cheats were allowed but never used.
- Added [Show Odner's explosion range] under Difficulty Relief (off by default).

## 1.43.0

- Shows which inventory slots the Mystic combo will double before you pick up any Mystic artifact (off by default).

## 1.42.0

- The inventory in the run history can be scrolled.
- PgUp/PgDn moves the in-game inventory one row at a time.
- Reroll limits can be set per reward type.
- Spawn, health and damage multipliers can be typed in up to 10000x.
- Draws a line to other players' pings.
- Removed the talent mirror from town.
- Mod-granted inventory slots are no longer reclaimed while they still hold an item.

## 1.41.0

- With [Hold to keep dashing] on, holding the key outside combat now gives the game's normal run.

## 1.40.2

- Fixed [Friendly allies] removing the blood-donation bat, which made the event disappear.

## 1.40.1

- Fixed color and line-spacing tags showing as raw text in the party status panel.

## 1.40.0

- Added [Keep concurrent enemy limit unscaled] to enemy settings (off by default).
- Added [Gain EXP and leaves instantly] to run settings (off by default).
- Added [Spread drop spawning and processing] to run settings (off by default).

## 1.38.0

- Key binding rows now behave exactly like the game's own "Keyboard" options tab.
