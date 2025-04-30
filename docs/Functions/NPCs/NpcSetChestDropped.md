# NpcSetChestDropped

### Syntax

`NpcSetChestDropped(npc_id,chest_dropped);`

**Returns** nothing.

| **Argument**   | **Type** | **Description**                                       |
| :------------- | :------- | :---------------------------------------------------- |
| npc_id         | String   | The NPC ID that should be used.                      |
| chest_dropped | String   | The chest that this NPC should drop when it dies. |

Assigns the NPC a specific chest to drop.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Assign our NPC a chest to drop
NpcSetChestDropped("test_npc","human_master_normal")
```

The above code will create a NPC and then assign it to the "human_master_normal" chest to drop when it dies..