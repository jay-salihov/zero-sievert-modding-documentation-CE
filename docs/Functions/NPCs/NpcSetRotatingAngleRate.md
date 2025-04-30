# NpcSetRotatingAngleRate

### Syntax

`NpcSetRotatingAngleRate(npc_id,rotation_angle_maximum);`

**Returns** nothing.

| **Argument**          | **Type** | **Description**                                      |
| --------------------- | -------- | ---------------------------------------------------- |
| npc_id                | String   | The NPC ID that should be used.                      |
| rotation_angle_maximum | Real     | The maximum rate that the NPC can rotate per frame. |

When the NPC hits the player, there is a chance that their shot will be a full-hit, this modifies the likeliness of that.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Modifies the rate that the NPC can rotate per frame.
NpcSetRotatingAngleRate("test_npc",10)
```

The above code will create a NPC and then modifies their rotation angle rate.