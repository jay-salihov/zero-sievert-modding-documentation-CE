# ChestSetIsDrop

### Syntax

`ChestSetIsDrop(chest_id,is_drop);`

**Returns** undefined.

| **Argument** | **Type** | **Description** |
|---|---|---|
| chest_id | String | The chest ID to modify. |
| is_drop | Boolean | Whether or not this chest is a drop. |

Used to determine whether or not this chest is a drop.

### Example:

```
-- Create a chest
ChestCreate("new_chest")
-- Set chest to be a drop
ChestSetIsDrop("new_chest",true)
```

The above code creates a new chest and then sets chest to be a drop.