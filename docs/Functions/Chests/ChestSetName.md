# ChestSetName

### Syntax

`ChestSetName(chest_id,chest_name);`

**Returns** undefined.

| **Argument** | **Type** | **Description**              |
| :----------- | :------- | :------------------------- |
| chest_id     | String   | The chest ID to modify.    |
| chest_name   | String   | The name of the chest.     |

Sets the name of the chest which is displayed on the UI.

### Example:

```
-- Create a chest
ChestCreate("new_chest")
-- Rename the chest
ChestSetName("new_chest","New Chest")
```

The above code creates a new chest and then names it.