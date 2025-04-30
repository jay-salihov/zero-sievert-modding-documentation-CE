# ItemBackpackSetMovementSpeed

### Syntax

`ItemBackpackSetMovementSpeed(item_id, movement_speed);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                        |
| :----------- | :------- | :----------------------------------------------------- |
| item_id      | String   | The name of the item to update.                        |
| movement_speed | Real     | When equipped how much to change players move speed stat. |

This is used to alter the move speed stat of the player. This value should normally be between -15 and 15. Negative numbers reduce a players speed, positive numbers increase the players move speed.