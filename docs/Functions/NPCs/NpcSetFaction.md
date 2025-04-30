# NpcSetFaction

### Syntax

`NpcSetFaction(npc_id,faction);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| npc_id       | String   | The NPC ID that should be used.              |
| faction      | String   | The faction that this NPC belongs to. |

Assigns the NPC to a specific faction.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Assign our NPC a faction
NpcSetFaction("test_npc","Bandits")
```

The above code will create a NPC and then assign it to the "Bandits" faction.