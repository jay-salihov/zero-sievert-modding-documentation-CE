# ItemMedicalSetWound

### Syntax

`ItemMedicalSetWound(item_id, wound);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| item_id      | String   | The name of the item to update.               |
| wound        | Real     | Amount of Wound to remove.                    |

If the player has stacks of Wound this will remove this amount.

Please note: *This actually accepts negative numbers which will actually put stacks of Wound onto the player.*

### Example:

```
-- Create our medical item
ItemMedicalCreate("Daves Wound Removal Gel",0)
ItemMedicalSetWound("Daves Wound Removal Gel",1)
```

This would create a new item that can be spawned into the game that when consumed will remove 1 stack of Wound from the player.