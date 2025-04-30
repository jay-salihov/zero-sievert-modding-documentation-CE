# ItemSetDescription

### Syntax

`ItemSetDescription(item_id, item_description);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| item_id      | String   | The name of the item to adjust.               |
| item_description | String   | A description shown ingame for this item. |

Changes the description shown ingame for this item.

### Example:

```
-- Modify the description of the bandage item 
ItemSetDescription("bandage", "This is a nice item, especially when you are bleeding") 
```

The above code will change the description of the bandage item.