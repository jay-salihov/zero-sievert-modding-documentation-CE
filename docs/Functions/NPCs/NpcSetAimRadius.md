# NpcSetAimRadius

### Syntax

`NpcSetAimRadius(npc_id,radius_minimum,radius_maximum);`

**Returns** nothing.

| **Argument**           | **Type** | **Description**                                     |
| ---------------------- | -------- | --------------------------------------------------- |
| npc_id                 | String   | The NPC ID that should be used.                    |
| recoil_radius_minimum  | Real     | The minimum radius that is aimed inside of.        |
| recal_radius_maximum   | Real     | The maximum radius that is aimed inside of.        |

When the NPC shoots the white circle (seen below) increases in radius to simulate the recoil. It can go from `recoil_radius_minimum` to `recal_radius_maximum`. The bigger the radius, the more likely that the NPC misses their shot.

<span><img/></span>

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Modifies the recoil aim radius
NpcSetAimRadius("test_npc",15,60)
```

The above code will create a NPC and then modifies their recoil radius.