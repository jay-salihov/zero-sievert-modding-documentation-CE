# NpcCopy

### Syntax

`NpcCopy(npc_id,npc_id_to_copy);`

**Returns** nothing.

| **Argument**      | **Type** | **Description**                             |
| ------------------- | -------- | ------------------------------------------- |
| npc_id            | String   | The NPC ID that should be copied to.        |
| npc_id_to_copy | String   | The NPC ID to copy from.                    |

This can be used to copy NPC data from one to another. It creates a unique copy meaning that changing one NPC won't modify the other. This feature is helpful if you want to create a NPC that has identical behavior to the Barman for example, but want a different `speaker_id`.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Copy our NPCs data from the data used for the Barman
NPCcopy("test_npc","barman")
```

The above code will create a NPC with the specified ID and then copy the Barman's data over it.