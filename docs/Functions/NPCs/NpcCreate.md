# NpcCreate

### Syntax

`NpcCreate(npc_id);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| npc_id       | String   | The NPC ID that will be used for reference later. |

Creates an NPC that is a clone of the "loner_novice" NPC by default. This NPC can be referred to later with the specified ID.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")
```

The above code will create a NPC with the specified ID.