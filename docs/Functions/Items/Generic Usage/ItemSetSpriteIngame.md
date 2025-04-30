# ItemSetSpriteIngame

### Syntax

`ItemSetSpriteIngame(item_id, sprite_name);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                    |
| :----------- | :------- | :------------------------------------------------- |
| item_id      | String   | The name of the item to assign the sprite to.      |
| sprite_name  | String   | A name to use as a reference to the sprite. |

Assigns a sprite you’ve loaded to an asset in the game. You can assign sprites to new items that have been added or items that already exist. This replaces the ingame sprite specifically. For example the sprite for guns in the world compared to the inventory.

### Example:

```
-- Assign our sprite to the "bandage" item asset
ItemSetSpriteIngame("bandage", "test_item")
```

The above code will assign a sprite to be used as the sprite for the bandage when displayed in the inventory.