# SpriteSetOrigin

### Syntax

`SpriteSetOrigin(sprite_name,x,y);`

**Returns** the sprite if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
|--------------|----------|-----------------------------------------------|
| sprite_name  | String   | The name of the sprite to modify the origins of. |
| x            | Real     | The x position for the origin.                |
| y            | Real     | The y position for the origin.                |

You can change the origin positions for sprites. This is the point from which the sprite is centered from.

### Example:

```
-- Load our item sprite
SpriteLoad("test_item","test_item.png",1,0,0,0);
-- Now modify the origins of this sprite
SpriteSetOrigin("test_item",10,10)
```

The above code will load our image and modify it's sprite origins.