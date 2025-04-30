# ItemBackpackSetSpriteGame

### Syntax

`ItemBackpackSetSpriteGame(item_id, sprite);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| item_id      | String   | The name of the item to assign the sprite to.   |
| sprite       | Real     | What sprite should be displayed when this item is equipped. |

The sprite must already be made using SpriteLoad()

### Example:

```
SpriteLoad("daves_big_backpack","world_backpack_image.png",1,0,0,0) 
ItemBackpackSetSpriteGame("daves_backpack", "daves_big_backpack") 
```

The above code will change the item called "daves_backpack" so that when its being worn the `world_backpack_image.png` will be drawn on the player.