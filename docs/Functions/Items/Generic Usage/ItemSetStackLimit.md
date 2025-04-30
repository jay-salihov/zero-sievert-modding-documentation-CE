# ItemSetStackLimit

### Syntax

`ItemSetStackLimit(item_id, stack_limit);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| item_id      | String   | The name of the item to adjust.               |
| stack_limit  | Real     | The stack limit for this item.                |

Changes the stack limit of this item.

### Example:

```
-- Modify the stack limit of the bandage item
ItemSetStackLimit("bandage", 100)
```

The above code will change the stack limit of the bandage item to 100.