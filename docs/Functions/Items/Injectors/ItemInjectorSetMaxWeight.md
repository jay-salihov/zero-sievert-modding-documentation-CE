# ItemInjectorSetMaxWeight

### Syntax

`ItemInjectorSetMaxWeight(item_id, max_weight);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| item_id      | String   | The name of the item to update.                  |
| max_weight   | Real     | Amount to change the players carry weight |

While the Injector is active how much to change the amount the player can carry.

Note: *This could be a negative number to reduce the players max carry weight.*