# NpcSetImageSpeed

### Syntax

`NpcSetImageSpeed(npc_id,idle_animation_speed,moving_animation_speed);`

**Returns** nothing.

| **Argument**          | **Type** | **Description**                                  |
| --------------------- | -------- | ------------------------------------------------ |
| npc_id              | String   | The NPC ID that should be used.                  |
| idle_animation_speed | Real     | The animation speed used when the NPC is idle.   |
| moving_animation_speed | Real     | The animation speed used when the NPC is moving. |

Modifies the animation speed for the NPC in both the idle and the moving state.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Modify the animation speed of our NPC
NpcSetImageSpeed("test_npc",0.1,0.2)
```

The above code will create a NPC and then modify its animation speed.