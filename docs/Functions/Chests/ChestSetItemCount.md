# ChestSetItemCount

### Syntax

`ChestSetItemCount(chest_id,minimum_item_count,maximum_item_count);`

**Returns** undefined.

| Argument           | Type   | Description                                         |
| ------------------ | ------ | --------------------------------------------------- |
| chest_id           | String | The chest ID to modify.                             |
| minimum_item_count | Real   | The minimum number of items in the chest.           |
| maximum_item_count | Real   | The maximum number of items in the chest.           |

Sets the number of items that will spawn in a chest. It chooses a random amount from somewhere between the minimum and maximum values.

### Example:

```
-- Create a chest
ChestCreate("new_chest")

-- Set the number of items that spawn in the chest between 10 and 30
ChestSetItemCount("new_chest",10,30)
```

The above code creates a new chest and then sets the number of items that spawn in it between 10 and 30.