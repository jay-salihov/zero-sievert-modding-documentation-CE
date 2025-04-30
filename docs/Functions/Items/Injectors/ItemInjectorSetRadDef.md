# ItemInjectorSetRadDef

### Syntax

`ItemInjectorSetRadDef(item_id, rad_def);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                                     |
| :----------- | :------- | :------------------------------------------------------------------ |
| item_id      | String   | The name of the item to update.                                     |
| rad_def      | Real     | Gives a defence to Radiation during the duration of this injector. |

This adjusts the amount of damage from radiation the player gets while this injector is active. Just like some armours give defence against radiation damage this will work the same.

Note: *This could be a negative number to make the player gain more radiation but we don't recommend it.*