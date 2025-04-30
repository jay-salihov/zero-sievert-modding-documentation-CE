# ItemInjectorSetRadRegen

### Syntax

`ItemInjectorSetRadRegen(item_id, rad_regen);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                                                                                                                                                                                                                                          |
| :----------- | :------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| item_id      | String   | The name of the item to update.                                                                                                                                                                                                                                        |
| rad_regen    | Real     | Amount of Radiation to recover between now and the duration of the injector.                                                                                                                                                                                            |

The can be used to set if the injector recovers Radiation over time.

Please note: Because this is related to the Duration having a smaller Duration would mean the player recovers more Radiation every second and conversely longer Durations would make it so the injector recovers less Radiation a second.

Note: *This could be a negative number to give the player radiation but we don't recommend it.*