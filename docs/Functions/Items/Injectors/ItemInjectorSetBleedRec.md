# ItemInjectorSetBleedRec

### Syntax

`ItemInjectorSetBleedRec(item_id, bleed_rec);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| item_id      | String   | The name of the item to update.               |
| bleed_rec    | Real     | number of stacks to recover (default 0)       |

The can be used to set if the injector recovers Bleed.

Note: *This could be a negative number to give Bleed but this isn't recommended.*