# ChestSetSprite

### Syntax

`ChestSetSprite(chest_id,sprite);`

**Returns** undefined.

| **Argument** | **Type** | **Description** |
|---|---|---|
| chest_id | String | The chest ID to modify. |
| sprite | String | The sprite used for the chest. |

Sets the sprite that is used for the chest.

### Example:

```
-- Create a chest
ChestCreate("new_chest")
-- Sets the chest sprite
ChestSetSprite("new_chest","chest_sprite")
```

The above code creates a new chest and then assign it a sprite.