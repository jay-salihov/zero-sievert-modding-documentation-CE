# ItemInjectorSetHpRegen

### Syntax

`ItemInjectorSetHpRegen(item_id, hp_regen);`

**Returns** “*<strong>true</strong></em>“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                                                                                                                                             |
| :----------- | :------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| item_id      | String   | The name of the item to update.                                                                                                                                              |
| hp_regen     | Real     | Amount of HP to get back between now and the duration of the injector.                                                                                                       |

The can be used to set if the injector gives the player HP over time.

Please note: Because this is related to the Duration having a smaller Duration would mean you get more HP back every second and conversely longer Durations would make it so the injector gives less HP a second.

Note: *This could be a negative number to lose HP but this isn't recommended.*