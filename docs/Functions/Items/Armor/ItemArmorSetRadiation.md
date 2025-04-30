# ItemArmorSetRadiation

### Syntax

`ItemArmorSetRadiation(item_id, radiation);`

**Returns** "*true*", if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                                   |
|--------------|----------|-------------------------------------------------------------------|
| item_id      | String   | The name of the item to update.                                  |
| radiation    | Real     | How much protection from radiation does this armor give you |

This reduces the damage taken by radiation when this armor is equipped. We expect this to be a number between 0 and 200 with 200 reducing the radiation by the greatest amount.