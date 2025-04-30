# NpcSetHp

### Syntax

`NpcSetHp(npc_id,hp);`

**Returns** nothing.

| **Argument** | **Type** | **Description** |
|---|---|---|
| npc_id | String | The NPC ID that should be used. |
| hp | Real | The health value for the NPC. |

Sets the health value for a NPC.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Set the HP for the NPC
NpcSetHp("test_npc",50)
```

The above code will create a NPC and then sets its health to 50.