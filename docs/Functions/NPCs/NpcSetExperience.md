# NpcSetExperience

### Syntax

`NpcSetExperience(npc_id,experience);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                        |
| :----------- | :------- | :----------------------------------------------------- |
| npc_id       | String   | The NPC ID that should be used.                       |
| experience   | Real     | The amount of experience that this NPC is worth when killed. |

Sets the experience provided by an NPC when defeated.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")
-- Set the experience provided by killing this NPC
NpcSetExperience("test_npc",30)
```

The above code will create a NPC and then sets the experience this NPC provides to 30.