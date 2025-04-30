# ItemMedicalSetMoveSpeedMultiplier

### Syntax

`ItemMedicalSetMoveSpeedMultiplier(item_id, speed_multiplier);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                    |
| :----------- | :------- | :------------------------------------- |
| item_id      | String   | The name of the item to update.        |
| speed_multiplier | Real     | Change in move speed. |

While this item is being consumed this changes the move speed.

Note: This accepts numbers greater than 1 which would make the player move faster.

### Example:

```
-- Create our medical item
ItemMedicalCreate("Daves Healing Gel",50)
ItemMedicalSetDuration("Daves Healing Gel",60)
ItemMedicalSetMoveSpeedMultiplier("Daves Healing Gel", 0.5);
```

This would make an item heals 50 HP when used and for 60 frames (1 second) the player will move at half speed.