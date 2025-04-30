# Game Events

You can assign functions to be called during certain game events.

| **Event ID** | **Description**                                                                                                 |
| :----------- | :-------------------------------------------------------------------------------------------------------------- |
| "enter_hub"  | Called once when the hub room is entered. This means when you start a new game/load a save, or return from a raid. |
| "enter_raid" | Called once when the raid is started. Specifically this runs right after you continue past the loading screen. |
| "player_spawn" | Called once when the player spawns into the world. This will occur when you first enter any (Game Maker) room/level. |
| "player_death" | Called once when the player dies during raids.                                                                  |
| "trade_completed" | Whenever the player successfully completes a trade with a trader.                                               |