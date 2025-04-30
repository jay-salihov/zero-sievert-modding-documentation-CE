# ItemMedicalSetBleed

### Syntax

`ItemMedicalSetBleed(item_id, bleed);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                     |
| :----------- | :------- | :------------------------------------ |
| item_id      | String   | The name of the item to update.       |
| bleed        | Real     | Amount of Bleed to remove.            |

If the player has stacks of Bleed this will remove this amount.

Please note: *This actually accepts negative numbers which will actually put stacks of Bleed onto the player.*

### Example:

```
-- Create our medical item
ItemMedicalCreate("Daves Bleed Removal Gel",0)
ItemMedicalSetBleed("Daves Bleed Removal Gel",1)
```

This would create a new item that can be spawned into the game that when consumed will remove 1 stack of Bleed from the player.