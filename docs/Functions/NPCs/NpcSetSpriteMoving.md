# NpcSetSpriteMoving

### Syntax

`NpcSetSpriteMoving(npc_id,sprite);`

**Returns** nothing.

| **Argument** | **Type**   | **Description**                                                              |
| :----------- | :--------- | :--------------------------------------------------------------------------- |
| npc_id       | String     | The NPC ID that should be used.                                             |
| sprite       | String/Real | The name of the sprite or the reference to a sprite returned by [SpriteGet](SpriteGet). |

Assigns a sprite to be used when the NPC is in a moving state.

### Example:

```lua
-- Create our NPC
NpcCreate("test_npc")

-- Assign our NPC a moving sprite
NpcSetSpriteMoving("test_npc","test_npc_moving")
```

The above code will create a NPC and then assigns it a sprite to use for its moving state.