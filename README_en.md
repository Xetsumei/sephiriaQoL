# Sephiria QoL Mod

**Sephiria QoL** is a comprehensive mod that adds various **quality-of-life features, difficulty adjustments, and other cheat-like features** not natively supported by Sephiria. It is designed for single-player or **multiplayer with other users of the same QoL mod**.

When all features are disabled, the game is designed to behave exactly like the vanilla version.

> **Multiplayer Notice**
> Because the QoL mod includes cheat-like features, using it indiscriminately in multiplayer may be considered hacking. Therefore, **multiplayer with vanilla users is restricted by default**.
> * **When you are the host:** The room title is prefixed with `[QoL]`, and vanilla users are automatically kicked if they join.
> * **When you are a guest:** If you join a vanilla host's room, the message `[Mod] Sephiria QoL is enabled.` is posted in chat. If full QoL functionality is enabled, you automatically leave the room. (The host's settings take precedence.)

---

## Installation

1. Extract the contents of the downloaded archive into the AddOns folder inside your Sephiria installation directory.
2. The path should look like this:
   `.../Sephiria/AddOns/SephiriaQoL/SephiriaQol.dll`
3. **Important:** The `Libs` folder must also be present in the same directory for the mod to work properly!

<img width="394" height="199" alt="image" src="https://github.com/user-attachments/assets/adeca4bc-74d6-486e-8807-376b18a8f211" />

---

## Configuring Options

Press `ESC` during the game to open the **pause menu**. You will find a new **[QoL Settings]** tab at the top.

<img width="739" height="804" alt="image" src="https://github.com/user-attachments/assets/0f6b618a-b376-4010-a474-622e3dad7902" />

---

## General Settings and Features

<img width="850" height="94" alt="image" src="https://github.com/user-attachments/assets/4f18a54b-0f95-4559-b1b4-ba62daeef153" />

### QoL Mode Status
The mod has 3 operating modes to suit different play styles.

* **QoL Features Off:** Makes the game behave exactly like the vanilla version.
* **QoL Features On:** Enables all features. (Multiplayer with vanilla users is restricted.)
* **QoL Features: Convenience Only:** Enables only pure convenience features, with no cheat-like functionality. In this mode, multiplayer with vanilla users is not restricted, but a chat message announces that QoL features are enabled when a run begins.

 <img width="850" height="59" alt="image" src="https://github.com/user-attachments/assets/479e0a73-7630-4c8c-8a60-09ca66e0f163" />

#### Options Allowed in Convenience-Only Mode
> ★ marks **host-only** features. They work only when you are the host and also apply to guests who do not have the mod. When you are a guest, changing a multiplier does not affect the host.

**<General>**
* Hold to auto-cast magic
* Hold to auto-cast special attacks
* Expand preset slots to 100

**<Enemies>**
* ★ Enemy spawn multiplier / per-floor settings
* ★ Enemy health multiplier / per-floor settings / per-type settings
* ★ Ease Blood Festival
* ★ Apply the spawn multiplier to mid-bosses
* ★ Enemy damage multiplier settings
* ★ Enemy pattern speed settings

**<Run>**
* Instant reroll button
* ★ Inventory slot per level-up
* ★ Leaf / EXP gain multipliers
* ★ Grant leaves at the start of the game
* ★ Share the lucky medal effect (guests receive gold only)
* ★ Share the party's highest negotiation / leaf gain / EXP gain values
* ★ Share potion pickups
* ★ Multiplayer party size
* Notify when a secret room exists
* ★ Guarantee an anvil in the first choice

**<Difficulty Relief>**
* ★ Fixed enchant count

**<Display>**
* Party status panel settings
* Disable other players' pings

---

### Presets
Because the QoL mod has many configurable options, it includes recommended default presets from the creator (Easy/Normal/Hard/Very Hard). Changing any setting manually switches the preset status to 'Custom'.

<img width="850" height="137" alt="image" src="https://github.com/user-attachments/assets/37e9cec8-405e-4832-958e-6664d8a4099d" />

**Saving and Loading Personal Presets (Chat Commands)**
* Save: `/qol save 1~9`
* Load: `/qol load 1~9`

### Other Convenience Features
* **Auto-Cast Magic/Special Attacks:** Hold down the input for magic or an activatable artifact to cast it automatically whenever its cooldown ends. (Includes instant special attacks.)
* **Journal Search:** Search for entries by name in the journal.

<img width="584" height="81" alt="image" src="https://github.com/user-attachments/assets/7cc5a8d5-5999-4c09-9007-d86bc5fb9b58" />


* **View QoL Information:** Open the `ESC` pause menu to view real-time information about the QoL options applied to the current run.

<img width="849" height="529" alt="image" src="https://github.com/user-attachments/assets/abd8b68c-4720-476c-b55f-6b5e47989bd2" />

---

## Enemy Settings

<img width="849" height="282" alt="image" src="https://github.com/user-attachments/assets/dcedbba9-b07d-41c2-991e-32e67217ba2a" />

* **Enemy Spawn Multiplier:** Sets the number of enemies spawned as a multiplier. (Command: `/spawnrate number` or `/s number`)
* **Enemy Spawn Multiplier by Floor:** Sets the spawn multiplier separately for each of floors 1~6. (Command: `/s number floor`)
* **Enemy Health Multiplier:** Increases enemy health. For hack-and-slash gameplay, it also provides the options 'Reduce health by the spawn multiplier', '1/4x', and '1/2x'.
* **Ease Blood Festival:** Even when the enemy health multiplier is enabled, this forces life steal to be calculated using only each monster's 'base maximum health'.
* **Apply Multipliers to Mid-Bosses:**
  * **Spawn Multiplier:** Spawns as many copies of each mid-boss as specified by the spawn multiplier.
  * **Health Multiplier:** Mid-bosses already have a lot of health, so applying the full multiplier can make them take far too long to defeat. To avoid this, you can balance their bonus health by reducing it to 1/2 or 1/4, or by selecting 'Divide by spawn multiplier'.
* **Enemy Damage Multiplier / Pattern Speed:** Adjusts enemy damage and shortens pattern cooldowns to increase attack frequency.

---

## Run Settings

* **Game Speed:** Adjusts the game speed from 0.5x ~ 2x. (Limited to prevent lag; not applied in multiplayer.)
* **Inventory Columns:** Changes the inventory width from the default 6 slots to 1~10 slots. (Experimental feature.)
* **Sapphire Reroll System Rework:**
  > This option is intended to reduce repetitive currency farming (grinding), which detracts from the essence of a roguelike.
  > It fixes the reroll price at 0 while allowing you to **limit the number of rerolls** to prevent guaranteed items through unlimited rerolling. (Can be configured to suit either cheat-enabled or restricted play.)
* **Remove Level Cap:** Raises the maximum level to around level 1000, effectively removing the limit.
* **Inventory Slot per Level-Up:** Grants 1 inventory slot every n levels. (Intended to ease high-difficulty runs.)
* **Revive Speed Multiplier:** Adjusts the speed at which teammates are revived in multiplayer from 0.1x ~ 10x.

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
* **Expanded Party Size:** Increases the maximum multiplayer party size to 16. (UI elements may overlap.)

### Luck/Object Adjustments
* **Guarantee an Anvil in the First Room:** Always spawns an anvil in the first room of floor 1 or floor 2.
* **Secret Room Notification:** Notifies you when a secret room exists on the map.
* **Obelisk Rerolls:** Spend 1 die to reroll an obelisk reward.
* **Allow Bonded Artifacts:** Allows Bonded artifacts to be obtained from the wishing fountain.
* **Journal Ban Feature:** Wheel-click artifacts/tablets/weapons/miracles in the journal to ban them from appearing. (Commands: `/qol ban all`, `/qol ban off`)

<img width="850" height="248" alt="image" src="https://github.com/user-attachments/assets/7d9891b4-a796-4fde-923f-e91feb07c15f" />

* **Guarantee Special Objects:** Forces an obelisk, suspicious merchant, pocket dimension shop, and blood donation event to appear after defeating the boss on each floor.

<img width="850" height="599" alt="image" src="https://github.com/user-attachments/assets/7cba1c05-091c-4035-aaab-5808b0694c6d" />

---

## Difficulty Relief (Cheat Features)

These options explicitly make the game easier.

* **Reveal Minimap:** Immediately reveals the entire map, including secret rooms and exits, and enables fast travel.
* **Extra Reward Choices and Chests:** Increases the number of choices for artifacts, inventory, the wishing fountain, fruit skewers, talent points, dice, and more. (The chest multiplier is applied when a boss is defeated.)
* **Shop Relief:** Increases both the number of items merchants sell and the number of items added by rerolling.
* **Fixed Enchant Count:** Fixes the number of enchants that appear in enchantment rooms.
* **Hard-Mode Reward Unlock Relief:** If a player has not unlocked many hard-mode rewards, clearing a high tier (60) unlocks all rewards through level 50 at once.
* **Remove Unique-Effect Restrictions:** Allows duplicate artifacts with unique effects to be obtained so their effects can stack. (Does not work with some artifacts.)
* **Sapphire/Dice Cheats:**
  * The host can decide whether guests are allowed to use currency cheats in the room.
  * When enabled, sapphires are fixed at 999,999 and dice at 999.
  * Use the command `/qol sapphire rest` to set sapphires to 0.

  In other words, with these two features,

  "Cheats are banned in my room."
  "Cheats are allowed in my room, but I won't use them."
  "Cheats are allowed in my room, and I will use them too." are possible, but

  "I can cheat in my room, but you can't." is not.

<img width="457" height="80" alt="image" src="https://github.com/user-attachments/assets/30412622-0727-44eb-b016-ca6ecf987f69" />

---

## Display

* **Party Status Panel:** Displays each party member's cumulative damage, damage share (%), DPS, held currency (leaves/dice/sapphires), and TOP 3 combos. (When set to Custom, its position can be moved with `Alt + drag`.)
* **Disable Other Players' Pings:** Immediately blocks ping icons and sounds from other players.
* **Screen Scale (Zoom):** Zooms the game view out or in between 10% ~ 200%.
* **Colorblind Mode:** Independently enables 'Inventory Colorblind Mode' and 'Colorblind Mode for Attack Warnings', separate from the base game's settings.
  * **Commands (Change Attack Warning Color):**
    * `/qol colorblind <r> <g> <b>` (change to the desired RGB values)
    * `/qol colorblind reset` (reset to the default sky blue)
    * `/qol colorblind` (view the currently applied RGB values)
