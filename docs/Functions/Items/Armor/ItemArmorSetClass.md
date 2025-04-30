# ItemArmorSetClass

### Syntax

`ItemArmorSetClass(item_id, class);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| item_id      | String   | The name of the item to update.               |
| class        | Real     | Changes the class of this armor               |

The armour class changes what can be used to repair this armor. We expect this to be a value between 0 and 6. With 6 being the best armor.