# ItemMedicalSetDuration

### Syntax

`ItemMedicalSetDuration(item_id, duration);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                      |
| :----------- | :------- | :----------------------------------- |
| item_id      | String   | The name of the item to update.      |
| duration     | Real     | How long it takes to consume this item. |

This sets how long it will take to fully consume this item.

This is done in frames and the game runs at 60FPS. So setting this value to 30 will take half a second to consume and a value of 120 will take 2 second to consume.

When healing the amount is spread over this duration. So healing 90 HP over 60 frames would be healing at 1.5 HP a frame.

### Example:

```
-- Create our medical item
ItemMedicalCreate("Daves Healing Gel",50)
ItemMedicalSetDuration("Daves Healing Gel",60)
ItemMedicalSetCanMove("Daves Healing Gel", false);
```

This would make an item heals 50 HP over the course of 60 frames (1 second).