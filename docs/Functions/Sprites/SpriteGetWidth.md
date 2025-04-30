# SpriteGetWidth

### Syntax

`SpriteGetWidth(sprite_name);`

**Returns** the width of the sprite.

| **Argument** | **Type** | **Description**                                    |
| :----------- | :------- | :------------------------------------------------- |
| sprite_name  | String   | The name of the sprite to get. the width of. |

This can be used to get the width of a sprite.

### Example:

```
-- Load our item sprite
SpriteLoad("test_item","test_item.png",1,0,0,0);

let _sprite_width = SpriteGetWidth("test_item")
```

The above code will create a new sprite and then assign it's width to the variable, *_sprite_width*.