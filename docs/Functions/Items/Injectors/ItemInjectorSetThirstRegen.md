# ItemInjectorSetThirstRegen

### Syntax

`ItemInjectorSetThirstRegen(item_id, thirst_regen);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                                                                              |
| :----------- | :------- | :--------------------------------------------------------------------------------------------------------- |
| item_id      | String   | The name of the item to update.                                                                            |
| thirst_regen | Real     | Amount of Thirst to recover between now and the duration of the injector.                                  |

The can be used to set if the injector recovers Thirst over time.

Please note: Because this is related to the Duration having a smaller Duration would mean you get more Thirst back every second and conversely longer Durations would make it so the injector gives less Thirst a second.

Note: *This could be a negative number to reduce the players Thirst.*