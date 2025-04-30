# SpriteGet

### Syntax

`SpriteGet(sprite_name);`

**Returns** the sprite if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                  |
| :----------- | :------- | :----------------------------- |
| sprite_name  | String   | The name of the sprite to get. |

Gets a sprite that was previously added with [SpriteLoad](SpriteLoad). You will need to do this when assigning sprites to items, speakers, or anything else.

### Example:

```
-- Load our item sprite
SpriteLoad("test_item","test_item.png",1,0,0,0);
-- Now assign it to our "bandage" item asset
ItemSetSpriteInventory("bandage","test_item")
```

The above code will load our image and assign it to be used as the sprite for the bandage when displayed in the inventory.