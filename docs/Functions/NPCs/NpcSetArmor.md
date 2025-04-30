# NpcSetArmor

### Syntax

`NpcSetArmor(npc_id,armor);`

**Returns** nothing.

| **Argument** | **Type** | **Description** |
|---|---|---|
| npc_id | String | The NPC ID that should be used. |
| armor | String | The item ID of the armor this NPC should use. |

Assigns a specific item to a NPC to use as armor.

You can also use `no_item`.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Assign our NPC an armor to use
NpcSetArmor("test_npc","armor_loner_1")
```

The above code will create a NPC and then assign it the item "armor_loner_1" to use as armor.