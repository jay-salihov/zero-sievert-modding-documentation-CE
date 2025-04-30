# SpriteSetSpeed

### Syntax

`SpriteSetSpeed(sprite_name, framerate_multiplier);`

**Returns** false, otherwise it will crash.

| **Argument**         | **Type** | **Description**                               |
| -------------------- | -------- | --------------------------------------------- |
| sprite_name          | String   | The name of the sprite to get.                |
| framerate_multiplier | Real     | The value to multiply the framerate playback by. |

Sets the framerate speed for a sprite. A value of 0.25 would play the animation at 1/4th of the original rate.

### Example:

```
-- Load our npc sprite
SpriteLoad("test_npc_idle","test_npc_idle.png",3,0,0,0);

-- Now affect the sprite's framerate
SpriteSetSpeed("test_npc_idle",0.25)
```

The above code will load our image and assign it to be used as the sprite for the bandage when displayed in the inventory.