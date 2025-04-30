# NpcSetRecoilCrosshairDelay

### Syntax

`NpcSetRecoilCrosshairDelay(npc_id,delay);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| npc_id       | String   | The NPC ID that should be used.                 |
| delay        | Real     | The delay lerp value from 0 to 1.                |

When a NPC locks on to the player they follow their position with a small delay to simulate some sense of reflexes. This value is used in a lerp function (multiplicative).

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Modifies the recoil crosshair delay
NpcSetRecoilCrosshairDelay("test_npc",0.25)
```

The above code will create a NPC and then modifies its recoil crosshair delay value.