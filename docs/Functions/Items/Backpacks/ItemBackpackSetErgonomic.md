# ItemBackpackSetErgonomic

### Syntax

`ItemBackpackSetErgonomic(item_id, ergonomics);`

**Returns** “* **true** *“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                                                                                                                                                                                                                                                                           |
| :----------- | :------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| item_id      | String   | The name of the item to update.                                                                                                                                                                                                                                                                           |
| ergonomics   | Real     | When equipped how much to change players ergonomics stat.                                                                                                                                                                                                                                                |

This is used to alter the ergonomics stat of the player which changes recoil and cursor tracking speed. This value should normally be between -20 and 20. Negative numbers reduce a players effectiveness in recoil control, positive numbers will make recoil control easier.