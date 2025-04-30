# ItemSetName

### Syntax

`ItemSetName(item_id, item_name);`

**Returns** “* **true** *“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| item_id      | String   | The name of the item to adjust.               |
| item_name    | String   | A name shown ingame for this item.            |

Changes the ingame name of the item.

### Example:

```
-- Modify the ingame name of the bandage item 
ItemSetName("bandage", "healing tape") 
```

The above code will change the ingame name of the bandage item to "healing tape".