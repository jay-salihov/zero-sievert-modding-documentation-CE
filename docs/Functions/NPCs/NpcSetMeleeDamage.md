# NpcSetMeleeDamage

### Syntax

`NpcSetMeleeDamage(npc_id,melee_damage);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                                      |
| :----------- | :------- | :------------------------------------------------------------------- |
| npc_id       | String   | The NPC ID that should be used.                                     |
| melee_damage | Real     | The damage this NPC does when it melees. Only affects melee focused enemies. |

Sets the melee damage value for an NPC.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Set the melee damage for the NPC
NpcSetMeleeDamage("test_npc",50)
```

The above code will create a NPC and then sets melee damage to 50.