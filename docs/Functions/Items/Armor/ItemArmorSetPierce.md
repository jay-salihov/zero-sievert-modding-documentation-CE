# ItemArmorSetPierce

### Syntax

`ItemArmorSetPierce(item_id, pierce);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                  |
|--------------|----------|--------------------------------------------------|
| item_id      | String   | The name of the item to update.                  |
| pierce       | Real     | Reduce damage taken by melee attacks.            |

This reduces the damage taken by melee attacks when this armor is equipped. We expect this to be a number between 0 and 0.7 with 0.7 reducing the damage by the greatest amount.