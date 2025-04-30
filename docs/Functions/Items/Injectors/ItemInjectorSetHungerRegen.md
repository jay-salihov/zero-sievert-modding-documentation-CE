# ItemInjectorSetHungerRegen

### Syntax

`ItemInjectorSetHungerRegen(item_id, hunger_regen);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                                                                                                               |
| :----------- | :------- | :------------------------------------------------------------------------------------------------------------------------------------------ |
| item_id      | String   | The name of the item to update.                                                                                                           |
| hunger_regen | Real     | Amount of Hunger to recover between now and the duration of the injector.                                                                    |

The can be used to set if the injector recovers Hunger over time.

Please note: Because this is related to the Duration having a smaller Duration would mean you get more Hunger back every second and conversely longer Durations would make it so the injector gives less Hunger a second.

Note: *This could be a negative number to make the player more hungry.*