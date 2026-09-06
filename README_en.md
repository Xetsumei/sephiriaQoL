# Sephiria QoL Mod

**Sephiria QoL** is a comprehensive mod that adds various **quality-of-life features, difficulty adjustments, and other cheat-like features** not natively supported by Sephiria. It is designed for single-player or **multiplayer with other users of the same QoL mod**.

When all features are disabled, the game is designed to behave exactly like the vanilla version.

> **Multiplayer Notice**
> Because the QoL mod includes cheat-like features, using it indiscriminately in multiplayer may be considered hacking. With every feature turned on, **multiplayer with vanilla users is restricted by default**.
> * **When you are the host:** The room title is prefixed with `[QoL]`, and vanilla users are automatically kicked if they join.
> * **When you are a guest:** If you join a vanilla host's room, you automatically leave after 10 seconds.
> * If you want to play with vanilla users, use the **Convenience only** or **Convenience + host** modes described below. Neither is restricted.

---

## Installation

1. Extract the contents of the downloaded archive into the AddOns folder inside your Sephiria installation directory.
2. The path should look like this:
   `.../Sephiria/AddOns/SephiriaQoL/SephiriaQol.dll`
3. **Important:** The `Libs` folder must also be present in the same directory for the mod to work properly!

No separate loader has to be installed. The game's built-in add-on loader reads it as is.

<img width="394" height="199" alt="image" src="https://github.com/user-attachments/assets/adeca4bc-74d6-486e-8807-376b18a8f211" />

---

## Configuring Options

Press `ESC` during the game to open the **pause menu**. You will find three new entries: **[QoL Settings] · [QoL Info] · [QoL Run Log]**.

<img width="739" height="804" alt="image" src="https://github.com/user-attachments/assets/0f6b618a-b376-4010-a474-622e3dad7902" />

The settings window is split into five tabs, `General / Enemies / Run / Difficulty relief / Display`, and `Q` `E` (LB · RB on a gamepad) switch between them.

* **Sliders:** Rows with many steps, such as multipliers, have a slider attached.
* **Typing a number:** On any row with a slider you can click the value on the right and type the number directly. Type it exactly as the row shows it. (`1.5` → x1.5, `150` → 150%, `2000` → +2000 leaves)
  * Multiplier rows accept values that are not in the table, in steps of 0.1. Rows counted in slots, players or times snap to the nearest step.
* **Most rows are hidden during a run:** Anything that affects difficulty or rewards disappears once a run starts and comes back in the lobby. Changing the difficulty mid-run is effectively cheating.

---

## General Settings and Features

<img width="850" height="94" alt="image" src="https://github.com/user-attachments/assets/4f18a54b-0f95-4559-b1b4-ba62daeef153" />

### QoL Mode Status
The mod can operate in 4 modes to suit different play styles. What separates them is not difficulty but **where each feature is decided**.

* **Off:** Makes the game behave exactly like the vanilla version.
* **Convenience only:** Keeps only what starts and ends on your own screen and your own input. Nothing leaves your machine, so there is no room prefix, no chat notice and no mod handshake. From the outside you are indistinguishable from someone playing without the mod.
* **Convenience + host:** The above, plus everything **decided on the server**. These are features the host alone needs the mod for, so they apply to guests without the mod as well. Multiplayer with vanilla users is not restricted, but a chat message announces that QoL features are enabled when a run begins.
* **On:** Enables all features. Multiplayer with vanilla users is restricted.

You can also switch with `/qol on | host | solo | off`. This value alone is not affected by `/qol reset` or by presets.

 <img width="850" height="59" alt="image" src="https://github.com/user-attachments/assets/479e0a73-7630-4c8c-8a60-09ca66e0f163" />

#### Options that survive in Convenience only

**\<General\>**
* Hold to repeat-cast magic
* Hold to repeat special attack
* Expand preset slots to 100
* Put the talent mirror in town

**\<Run\>**
* Instant reroll button
* Multiplayer party size (your own cap has to be raised before you can join an expanded room, which is why it lives here. Turning it on does not widen a vanilla host's room.)

**\<Display\>**
* The whole tab, run log included.

Features that are not option rows, the journal name search and the QoL Info panel in the `ESC` menu, are available in this mode as well.

#### Options that additionally survive in Convenience + host
> Everything below applies **on the host's terms**. As the host it also affects guests without the mod; as a guest, changing these values has no effect on the run.

**\<General\>**
* QoL preset

**\<Enemies\>**
* All four multipliers: enemy spawn / health / damage / pattern speed (scope included)
* Ease Blood Festival
* Apply the spawn multiplier to mid-bosses

**\<Run\>**
* Inventory slot per level-up
* Leaf / EXP gain multipliers
* Extra starting leaf, extra starting dice
* Inventory columns
* Guarantee an anvil in the first choice, extra anvil
* Share lucky medal effect, share negotiation / leaf gain / EXP gain
* Share potion pickups
* Merchant durability, friendly allies
* Merchant always sells an inventory slot / EXP, mystic pot always appears

**\<Difficulty relief\>**
* Fix the enchant count
* Show every anvil enhancement
* Open the stats window / inventory during battle

What drops out here is anything **decided on a guest's machine that changes the run**: leaf and dice transfers, the wish fountain options, journal bans, removing the unique restriction, the cheats, obelisk rerolls, the reroll limit, game speed, revive speed, unlocking the level cap, free miracle rerolls, and the rest of the difficulty relief group. If the host alone turned those on, it is the guest without the mod who would break.

---

### Presets
Because the QoL mod has many configurable options, it includes recommended default presets from the creator (Easy/Normal/Hard/Expert). Changing any setting manually switches the preset status to 'Custom'.

<img width="850" height="137" alt="image" src="https://github.com/user-attachments/assets/37e9cec8-405e-4832-958e-6664d8a4099d" />

**Saving and Loading Personal Presets (Chat Commands)**
* Save: `/qol save 1~9`
* Load: `/qol load 1~9`
* List: `/qol list`

### Sharing Settings as a Code
You do not have to hand over the settings file itself.

* `/qol export` turns your current settings into a single line of text and puts it on the clipboard.
* The other person copies that code and types `/qol import`. `/qol import [code]` also works if they want to paste it in directly.

Only the settings you are currently using are exported. The nine slots are not included, and **display options, personal input options and journal bans are neither exported nor overwritten.**

### Other Convenience Features
* **Auto-Cast Magic/Special Attacks:** Hold down the input for magic or an activatable artifact to cast it automatically whenever its cooldown ends. (Includes instant special attacks.)
* **Journal Search:** Search for entries by name in the journal.

<img width="584" height="81" alt="image" src="https://github.com/user-attachments/assets/7cc5a8d5-5999-4c09-9007-d86bc5fb9b58" />

* **Put the Talent Mirror in Town:** Places a talent mirror in front of the dungeon entrance in the single-player town, so you no longer have to open and close a multiplayer room just to pick talents.
* **View QoL Information:** Open the `ESC` pause menu to view real-time information about the QoL options applied to the current run. As a guest it shows only the values actually received from the host.

<img width="849" height="529" alt="image" src="https://github.com/user-attachments/assets/abd8b68c-4720-476c-b55f-6b5e47989bd2" />

---

## Enemy Settings

<img width="849" height="282" alt="image" src="https://github.com/user-attachments/assets/dcedbba9-b07d-41c2-991e-32e67217ba2a" />

Spawn, health, damage and pattern speed all work the same way. Each multiplier row has a **scope** row under it that decides how finely that multiplier is split.

* **One value for everything:** A single value applies to all of it.
* **Per floor:** Floors 1~6 are set separately.
* **Per enemy type:** Normal enemies / mid-bosses / bosses are set separately.
* **Per floor and type:** The three types are set separately on each floor.

Values are kept per scope, so switching between scopes does not erase them.

* **Enemy Spawn Multiplier:** Sets the number of enemies spawned as a multiplier, from `1/4x` and `1/2x` up to `x100`. (Command: `/s number` or `/s number floor`)
* **Enemy Health Multiplier:** Adjusts enemy health. For hack-and-slash gameplay there are also `Reduce by the spawn multiplier` and `0.1x` ~ `0.9x`. (Command: `/h number` or `/h number floor`)
* **Enemy Damage Multiplier:** From `0.1x` up to `x100`, plus `Instant death`.
* **Enemy Pattern Speed:** Shortens pattern cooldowns to increase attack frequency. `0.5x` ~ `3x`.
* **Applying Multipliers to Mid-Bosses:** Mid-bosses spawn in the numbers set by the spawn multiplier. Their health is already high, so applying the multiplier in full makes them take far too long; use the per-type scope to lower mid-bosses on their own, or pick `Divide by the spawn multiplier`.
* **Ease Blood Festival:** Even when the enemy health multiplier is enabled, this forces life steal to be calculated using only each monster's 'base maximum health'.

From `x25` up the value is shown in red and a lag warning appears when you apply it. Commands accept up to 999x.

---

## Run Settings

* **Game Speed:** Adjusts the game speed from 0.5x ~ 2x. In multiplayer **everyone uses the host's value.** (Works only in an `On` room, where everyone has the mod.)
* **Inventory Columns:** Changes the inventory width from the default 6 slots to 1~10 slots.
* **Sapphire Reroll System Rework:**
  > This option is intended to reduce repetitive currency farming (grinding), which detracts from the essence of a roguelike.
  > It fixes the reroll price at 0 while allowing you to **limit the number of rerolls** to prevent guaranteed items through unlimited rerolling. (Can be configured to suit either cheat-enabled or restricted play.)
* **Instant Reroll Button:** Rolls immediately without having to hold the reroll button down.
* **Unlock Level Cap:** Raises the maximum level to around level 1000, effectively removing the limit.
* **Inventory Slot per Level-Up:** Grants 1 inventory slot every n levels. (Intended to ease high-difficulty runs.)
* **Revive Speed Multiplier:** Adjusts the speed at which teammates are revived in multiplayer from 0.1x ~ 10x.
* **Leaf / EXP Gain Multipliers:** Adjustable from x0.1 to x20.0 in steps of 0.1.

### Multiplayer-Specific Features
* **Currency Transfers:** Transfer leaves or dice to another player through chat. (An index number can be used instead of a nickname.)
  * Transfer leaves: `/giveleaf [nickname/index] [number]` (short form: `/gl`)
  * Transfer dice: `/givedice [nickname/index] [number]` (short form: `/gd`)
* **Starting Item Transfers:** Drop starting items obtained from the wishing fountain, talents, and similar sources so other players can pick them up.
* **Lucky Medal & Stat Sharing:**
  * Shares the lucky medal effect with party members.
  * Shares the party's highest negotiation, leaf gain, and EXP gain values.
* **Distribution (to Nerf Resource-Farming Builds):** Divides leaf/EXP gains **by the number of party members** to prevent currency-maximizing builds from becoming overpowered.
* **Share Potion Pickups:** Gives every party member 1 copy of a potion found in a field chest instead of awarding it only to the first player who picks it up.
* **Expanded Party Size:** Increases the maximum multiplayer party size to 16. (UI elements may overlap. The game balances EXP distribution around 4 players, so raise the EXP multiplier to compensate when going much higher.)

### Luck/Object Adjustments
* **Guarantee an Anvil in the First Room:** Always spawns an anvil in the first room of floor 1 or floor 2.
* **Extra Anvil:** Places 1~2 additional anvils at the start of a floor.
* **Obelisk Rerolls:** Spend 1 die to reroll an obelisk reward.
* **Unlock the Wish Fountain:** Lets you pick Bonded artifacts and the suspicious merchant's goods at the wishing fountain.
* **Stack Picks at the Wish Fountain:** Lets you take several copies of the same item. **Left click adds, right click removes**, and the count is shown in the top-left of the icon. Capacity and cost use the game's own math, so two copies cost twice as much. Unique artifacts are limited to one. (On a gamepad, the rotate-item button removes.)
* **Journal Ban Feature:** Wheel-click artifacts/tablets/weapons/miracles in the journal to ban them from appearing. During a run everyone follows the host's list. (Commands: `/qol ban all`, `/qol ban off`)

<img width="850" height="248" alt="image" src="https://github.com/user-attachments/assets/7d9891b4-a796-4fde-923f-e91feb07c15f" />

* **Guarantee Special Objects:** Forces an obelisk, suspicious merchant, pocket dimension shop, and blood donation event to appear after defeating the boss on each floor. (Floor 6 is not offered, since beating its boss ends the run.)

<img width="850" height="599" alt="image" src="https://github.com/user-attachments/assets/7cba1c05-091c-4035-aaab-5808b0694c6d" />

* **Guaranteed Merchant-Room Props:** The EXP barrel, inventory orb and mystic pot next to the merchant each roll their own chance and remove themselves. These options make each of them appear for certain.
* **Merchant Durability / Friendly Allies:** Stops an auto-attack build from accidentally hitting a merchant and turning it hostile, and stops friendly NPCs from being farmed for the currency they drop on death. Merchants can be set to `Invulnerable` or `Set health to 1`, friendly NPCs to `Remove from the map` or `Set health to 1`.

---

## Difficulty Relief (Cheat Features)

These options explicitly make the game easier.

* **Reveal Minimap:** Immediately reveals the entire map, including secret rooms and exits, and enables fast travel.
* **Extra Reward Choices and Chests:** Increases the number of artifacts, inventory slots, wishing fountain capacity, fruit skewers, talent points, starting leaves, dice and so on. (The chest multiplier is applied when a boss is defeated.)
* **Show Every Anvil Enhancement:** Shows every enhancement the anvil can offer.
* **Shop Relief:** Increases both the number of items merchants sell and the number of items added by rerolling.
* **Fix the Enchant Count:** Fixes the number of enchants that appear in enchantment rooms to a value between 1 and 10.
* **Free Miracle Rerolls:** Lets you keep rerolling miracles with no dice at all.
* **Open the Stats Window / Inventory During Battle:** Lets you open the character stats window and the inventory while a battle is running. Time keeps flowing, so you take hits with the window open.
* **Allow Engraving the Chintamani Stone:** The Chintamani Stone normally revives you once on death, leaves `+3` levels on the slot it occupied, and disappears. With this on, hold right-click on the stone in your bag to fill the same gauge as a stone-tablet engraving and take that second half early. The levels stay on the slot, so they also apply to whatever artifact you place there later.
* **Hard-Mode Reward Unlock Relief:** If a player has not unlocked many hard-mode rewards, clearing a high tier (60) unlocks all rewards through level 50 at once.
* **Remove Unique-Effect Restrictions:** Allows duplicate artifacts with unique effects to be obtained so their effects can stack. (Does not work with some artifacts.)
* **Sapphire/Dice Cheats:**
  * The host can decide whether guests are allowed to use currency cheats in the room.
  * When enabled, sapphires are fixed at 999,999 and dice at 999.
  * Use the command `/qol sapphire reset` to set sapphires to 0.

  In other words, with these two features,

  "Cheats are banned in my room."
  "Cheats are allowed in my room, but I won't use them."
  "Cheats are allowed in my room, and I will use them too." are possible, but

  "I can cheat in my room, but you can't." is not.

<img width="457" height="80" alt="image" src="https://github.com/user-attachments/assets/30412622-0727-44eb-b016-ca6ecf987f69" />

---

## Display

* **Party Status Panel:** Displays each party member's cumulative damage, damage share (%), DPS, held currency (leaves/dice/sapphires), and TOP 3 combos. Each item can be toggled on its own, and the position is either `Right` or `Custom` (moved with `Alt + drag`).
* **Screen Zoom:** Zooms the game view out or in between 10% and 200%.
* **Colorblind Mode:** Independently enables 'Colorblind mode for the inventory' and 'Colorblind mode for attack warnings', separate from the base game's settings.
  * **Commands (Change Attack Warning Color):**
    * `/qol colorblind <r> <g> <b>` (change to the desired RGB values)
    * `/qol colorblind reset` (reset to the default sky blue)
    * `/qol colorblind` (view the currently applied RGB values)
* **Dropped EXP and Leaf:** Draws dropped EXP and leaves faded (50% / 25% / invisible). They are easy to mistake for enemy projectiles on a busy screen. Only the drawing changes; picking them up is unaffected.
* **Show Boss HP Numbers:** Adds a number to the health bar of bosses and mid-bosses.
* **Show the Boss's Aggro Target:** Draws a matching outline on the boss and on the player it is targeting.
* **Show Enchant Count on Item Slots:** Writes `★2` in the bottom-right of an item's slot to show how many times it has been enchanted. Normally you have to hover each slot for the tooltip. (On by default.)
* **Notify When a Hidden Room Exists:** Prints one line when you enter a floor that has a secret room.
* **Hide Other Players' Pings:** Immediately blocks ping icons and sounds from other players.
* **Chat Log Scrollback:** With the chat box open, put the mouse over the log lines and use the wheel to look back through the last 200 lines.
* **Highlight Item Pickup Notices:** Paints the item name in the pickup log with its rarity color. An artifact that completes a Bonded pair right there gets a gold-to-green gradient instead.

### Run Log
The game gives you no way to revisit a finished run. The moment the result screen closes, that run's bag and damage numbers are gone. So the **last 30 runs** are copied to a file as the result screen opens.

View them with `ESC` → `QoL Run Log`, or `/qol runs`. Choose between `Off / Mine only / Everyone in the party`; the default is `Mine only`.

* Each entry keeps the outcome, last location, play time, level, weapon, miracles, damage dealt and taken, and the top damage sources.
* `Tab` moves to the **bag** page, which shows that run's inventory laid out exactly as it was; press it again for the **totals** page.
* `Enter` reopens **the game's own result screen** with that run in it. From there the `[Damage]` button opens that run's damage window.
* Controls: keyboard `← →` run, `↑ ↓` party member, `Tab` page, `Enter` details, `ESC` close; gamepad uses the D-pad, `Y`, `A` and `B`.
* Records are written to a single file on your machine and nothing is sent over the network. `/qol runs clear` erases them. (This cannot be undone.)

---

## Chat Commands

```
/help                              command help

/s <rate> [floor]                  enemy spawn multiplier   (/spawnrate)
/h <rate> [floor]                  enemy health multiplier  (/hprate)

/gl <name|index> <amount>          give leaves      (/giveleaf)
/gd <name|index> <amount>          give dice        (/givedice)
/cheat s | /cheat d                sapphire / dice cheat status

/qol on | host | solo | off        all / convenience+host / convenience only / off
/qol reset                         restore every setting to vanilla
/qol load easy|normal|hard|expert  apply a difficulty preset
/qol save <1~9> | load <1~9>       store into / load from a slot
/qol list                          show presets and slots
/qol export | import [code]        share settings as a code
/qol ban all | off                 ban / unban every artifact
/qol runs [clear]                  view / erase the run log
/qol speed                         show the game speed in effect and where it came from
/qol sapphire reset                set sapphires to 0
/qol colorblind <r> <g> <b>        set the attack warning color
```

Adding a floor to a multiplier command switches that multiplier to per-floor automatically; leaving it out uses the global value. Typing a command without a value shows the current setting.

Commands that change settings only work **in the lobby**. The read-only ones, `/qol list` `/qol export` `/qol runs` `/qol speed`, work during a run as well.
