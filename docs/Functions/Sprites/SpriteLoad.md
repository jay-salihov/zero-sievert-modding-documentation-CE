# SpriteLoad

### Syntax

`SpriteLoad(sprite_name, file_name, image_number=1, removeback=false, x_origin=0, y_origin=0);`

**Returns** the "*__sprite_name__*" that is provided if successful, otherwise it will crash.

| **Argument**   | **Type** | **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| :------------- | :------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| sprite_name    | String   | A name to use as a reference to the sprite.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| file_name      | String   | The name (a string file path) of the file to add.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| image_number   | Real     | Use to indicate the number of sub-images (1 for a single image or for a **\*.gif**).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| removeback     | Boolean  | Indicates whether to make all pixels with the background colour (left-bottom pixel) transparent.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| x_origin       | Real     | Indicate the x position of the origin in the sprite.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| y_origin       | Real     | Indicate the y position of the origin in the sprite.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

Loads an external sprite into the game to be used later with the "*__sprite_name__*" provided. The filetypes supported are **\*.png**, **\*.gif**, **\*.jpg/jpeg**.

By default all new sprites have their bounding boxes calculated automatically (the exact bounding box will depend on the size and transparency of the sprite), however you may wish to customize this, in which case you should also use the function *__SpriteSetCollisionMask__*.

All the file paths are sandboxed and localized to the mod folder itself meaning you only need to provide the path from the root of the mod folder onward.

To later use this sprite you will need to use [SpriteGet](SpriteGet).

### Example:

```
-- Load our item sprite
SpriteLoad("test_item","test_item.png",1,0,0,0);

-- Now assign it to our "bandage" item asset
ItemSpriteSetInventory("bandage","test_item")
```

The above code will load our image and assign it to be used as the sprite for the bandage when displayed in the inventory.