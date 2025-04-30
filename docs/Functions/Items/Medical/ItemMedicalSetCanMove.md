# ItemMedicalSetCanMove

### Syntax

`ItemMedicalSetCanMove(item_id, can_move);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description** |
|---|---|---|
| item_id | String | The name of the item to update. |
| can_move | Boolean | When consuming this item can the player move? |

Sets if the player is able to move while this item is being consumed.

### Example:

```
-- Create our medical item
ItemMedicalCreate("Daves Healing Gel",50)
ItemMedicalSetDuration("Daves Healing Gel",60)
ItemMedicalSetCanMove("Daves Healing Gel", false);
```

This would make an item heals 50 HP when used and for 60 frames (1 second) the player will not be able to move.