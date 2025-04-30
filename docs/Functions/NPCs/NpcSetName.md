# NpcSetName

### Syntax

`NpcSetName(npc_id,name);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                     |
| :----------- | :------- | :------------------------------------ |
| npc_id       | String   | The NPC ID that should be used.      |
| trader_id    | String   | The trader ID that this NPC should use. |

Assigns a trader ID for this NPC to use.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")
-- Assign our NPC a name
NpcSetName("test_npc","Protagonist Guy")
```

The above code will create a NPC and then assign it the trader "test_trader".