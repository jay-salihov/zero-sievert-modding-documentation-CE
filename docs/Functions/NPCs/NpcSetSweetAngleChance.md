# NpcSetSweetAngleChance

### Syntax

`NpcSetSweetAngleChance(npc_id,sweet_angle_chance_minimum,sweet_angle_chance_maximum);`

**Returns** nothing.

| **Argument**             | **Type** | **Description**                                                           |
| ------------------------ | -------- | ------------------------------------------------------------------------- |
| npc_id                   | String   | The NPC ID that should be used.                                           |
| sweet_angle_chance_minimum | Real     | The minimum chance (0 to 1) for the NPC to get a full hit on the player. |
| sweet_angle_chance_maximum | Real     | The maximum chance (0 to 1) for the NPC to get a full hit on the player. |

When the NPC hits the player, there is a chance that their shot will be a full-hit, this modifies the likeliness of that.

### Example:

```lua
-- Create our NPC
NpcCreate("test_npc")

-- Modifies the chance of a full-hit from a sweet angle shot
NpcSetSweetAngleChance("test_npc",0.1,0.3)
```

The above code will create a NPC and then modifies their sweet angle chance.