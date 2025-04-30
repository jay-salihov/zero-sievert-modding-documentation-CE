# NpcSpawn

### Syntax

`NpcSpawn(npc_id, x, y);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| npc_id       | String   | The NPC ID that should be used.              |
| x            | Real     | The x position to spawn the NPC.              |
| y            | Real     | The y position to spawn the NPC.              |

Spawns an NPC into the world at a determined position. These NPCs should be created prior to this with [NpcCreate](NpcCreate).

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Spawn our NPC
NpcSpawn("test_npc",400,400)
```

The above code will create a NPC and then place it into the world.