# NpcObjectSpawnNearPlayer

### Syntax

`NpcObjectSpawnNearPlayer(npc_object, amount = 1, move_towards_player = false);`

**Returns** nothing.

| **Argument**          | **Type** | **Description**                                                                                                                              |
| --------------------- | -------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| npc_object            | String   | The npc object to spawn, use one of the ones from the enemy categories found on the [Pre-Existing Objects](Pre-Existing Objects) page. |
| amount                | Real     | The amount of NPCs to spawn near the player.                                                                                                 |
| move_towards_player | Real     | Whether the NPC should move towards the player after it spawns.                                                                               |

Spawns an NPC object on the edge of the player's view radius. The NPC objects can they move towards the player if `move_towards_player` is set to true.

### Example:

```
NpcObjectSpawnNearPlayer(obj_bandit_preset_rookie,3,true)
```

The above code will create 3 NPCs that will move towards the player.