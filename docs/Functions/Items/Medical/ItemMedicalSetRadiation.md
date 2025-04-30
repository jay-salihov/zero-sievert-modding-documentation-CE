# ItemMedicalSetRadiation

### Syntax

`ItemMedicalSetRadiation(item_id, radiation);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
|--------------|----------|-----------------------------------------------|
| item_id      | String   | The name of the item to update.               |
| radiation    | Real     | Amount of Radiation to remove.                |

If the player has stacks of Radiation this will remove this amount.

Please note: *This actually accepts negative numbers which will actually put stacks of Radiation onto the player.*

### Example:

```
-- Create our medical item
ItemMedicalCreate("Daves Radiation Removal Gel",0)
ItemMedicalSetRadiation("Daves Radiation Removal Gel",1)
```

This would create a new item that can be spawned into the game that when consumed will remove 1 stack of Radiation from the player.