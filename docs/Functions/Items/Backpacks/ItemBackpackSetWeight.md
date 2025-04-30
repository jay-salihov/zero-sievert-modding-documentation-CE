# ItemBackpackSetWeight

### Syntax

`ItemBackpackSetWeight(item_id, carry_weight);`

**Returns** “* **true** *“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                                                   |
| :----------- | :------- | :-------------------------------------------------------------------------------- |
| item_id      | String   | The name of the item to update.                                                   |
| carry_weight | Real     | When equipped the amount of weight the player can carry will be changed by this amount. |

Normally this value would be between 10 and 40 with 40 being the best value a bag should have.

Note: *This could be a negative number to make the player carry less (not advised).*