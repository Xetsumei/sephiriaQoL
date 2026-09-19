# Sephiria QoL — Patch notes

## 1.52.0 — 2026-09-19

- Fixed being thrown outside the map after visiting the shop through the portal from "Guarantee the pocket dimension". Instead of placing a portal on the spot, the mod now makes the floor generate the game's own pocket dimension room. It shows up on the minimap, and the return trip lands you where it should.
- The `Run rules` tab has a new "Guarantee the altar of luck" row below the other encounter guarantees. The chosen floor always gets a room with an altar of luck.
- Below it there is a new "Ban hidden room reward types" checkbox. Turning it on unfolds five rows — EXP chest, breakable pile, money chest, dice, mystic pot — and whatever you check will not appear in hidden rooms. You cannot check all five.
- "Ban hidden room reward types" applies to everyone in the room when the host turns it on. It cannot choose which hidden room appears, only what is placed inside it.
- Added a safety net for floor travel: when the game cannot find a landing spot it used to drop you outside the map, and now it sends you to that floor's starting point instead. This also covers runs that were started on 1.51.0 or earlier.

## 1.51.0 — 2026-09-18

- The `Relief` tab has a new "Free rerolls on the first level-up choice" checkbox, just above "Free miracle rerolls". With it on, the first level-up choice of a run can be rerolled without dice. Later level-up choices cost dice as usual.
- Only available when the QoL mode is `On`. When the host turns it on, it applies to everyone in the room.

## 1.50.1 — 2026-09-17

- Fixed items and tablets in the extra bottom slots added by "Extra inventory slots" disappearing when you quit the game and continued the run.

## 1.50.0 — 2026-09-16

- Fixed "Preview the slots the Mystic combo will double" pointing at the wrong slots after your inventory grew. In a room whose host has it on, Mystic slots are now fixed when the run starts, so they no longer move when you gain slots, and guests see the same slots.
- In the `Convenience only` tier only the preview runs, so the shown slots can still move when you gain slots.

## 1.49.2 — 2026-09-16

- Fixed "Auto special-then-basic attack" repeating only the special attack. The special and the basic attack now strictly alternate.
- The basic attack is now sent 0.1 seconds after the special, and the button is held until that attack starts — on weapons like the katana the follow-up cut only comes out while the button is still down.

## 1.49.1 — 2026-09-16

- "Auto dash-attack chain" now actually produces dash attacks. The basic attack used to go out first and bury the dash; while a dash is available the mod no longer lets a basic attack out, and repeats [dash → dash attack] instead. Basic attacks resume only while no dash is left.
- "Auto special-then-basic attack" now keeps chaining while left click is held. Only the first press used to get the special attack; now [special → basic] repeats for as long as the special attack is available.
- "Auto dash-attack chain" does nothing on weapons that have no dash attack (bow, staff, golem).

## 1.49.0 — 2026-09-16

- The [General] tab has a new "Auto dash-attack chain" checkbox. With it on, holding left click slips in a dash whenever one is ready, so dashes and basic attacks alternate.
- The [General] tab has a new "Auto special-then-basic attack" checkbox. With it on, every left click fires the special attack first and the basic attack follows. It covers the quarterstaff, dagger, katana and crossbow; the greatsword and sword-and-shield, which fire on button release, are excluded.
- Both are off by default, work in the `Convenience only` tier, and can be toggled during a run.

## 1.48.0 — 2026-09-16

- The `Relief` tab has a new "Enable stone tablet engraving from the start" checkbox. With it on, you can engrave tablets in your bag from the start of a run without reaching level 20 of the Survival talent.
- Only the host needs it on, and guests without the mod get it too.

## 1.47.5 — 2026-09-16

- The "Check for updates" row in the [General] tab is now a single "Automatic updates" checkbox.
- With it on, the mod checks for a new version every time you enter the game. It says "The mod is up to date." when there is nothing new, and opens the update window when there is.
- With it off, nothing is checked on launch and no update window appears. You can still check yourself with `/qol update`.

## 1.47.4 — 2026-09-16

- README and patch notes are available in the GitHub repository and are not included in release ZIPs.

- Updated the distribution files.


## 1.47.3 — 2026-09-16

- Updated the distribution files.


## 1.47.2 — 2026-09-15

- Release update history is available in the `patchlog` files.
- [Open patch notes] in the settings opens the patchlog for the game language.

## 1.47.1 — 2026-09-15

- Fixed an issue where cleanup could delete a newly installed version and prevent the mod from loading.
- Failed update checks no longer report that the mod is up to date.
- Restart is postponed if a run starts during the countdown. It also waits for other mod downloads.
- Automatic updates now refresh the README and update history.
- Update prompts from multiple mods no longer overwrite each other.

## 1.47.0

- When you enter the game, chat now shows the version check result: "The mod is up to date.", or, if a new version exists, the update prompt together with "You can update with /qol update."
- Mod notifications, command help and the update prompt now support Korean, English, Japanese and Chinese. They follow the game language; lines sent to the whole room's chat follow the host's language.
- The notification prefix changed from [모드] to [QoL].

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
