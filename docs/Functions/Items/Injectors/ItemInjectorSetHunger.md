# ItemInjectorSetHunger

### Syntax

`ItemInjectorSetHunger(item_id, hunger);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description** |
| ----------- | ----------- | ----------- |
| item_id | String | The name of the item to update. |
| hunger | Real | Amount of Hunger to recover. |

When the injector is used instantly change the Hunger by this amount. 

Note: *This could be a negative number to make the player more hungry.*