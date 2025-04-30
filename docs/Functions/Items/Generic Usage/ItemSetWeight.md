# ItemSetWeight

### Syntax

`ItemSetWeight(item_id, item_weight);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                       |
| :----------- | :------- | :------------------------------------ |
| item_id      | String   | The name of the item to adjust.       |
| item_weight  | Real     | The weight of the item.               |

Changes the weight of the item.

### Example:

```
-- Modify the weight of the bandage item
ItemSetWeight("bandage", 10)
```

The above code will change the weight of the item to weigh 10kg.