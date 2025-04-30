# ItemInjectorSetThirst

### Syntax

`ItemInjectorSetThirst(item_id, thirst);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description** |
| ----------- | ----------- | ----------- |
| item_id | String | The name of the item to update. |
| thirst | Real | Amount of Thirst to recover. |

When the injector is used instantly change the Thirst by this amount.

Note: *This could be a negative number to make the player more thirsty.*