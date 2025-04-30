# ItemArmorSetFragility

### Syntax

`ItemArmorSetFragility(item_id, fragility);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description** |
|---|---|---|
| item_id | String | The name of the item to update. |
| fragility | Real | How much damage this armor takes |

This changes how much durability this armor loses when taking damage. We expect this to be a number between 2 and 35