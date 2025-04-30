# ChestSetDestroyWhenEmpty

### Syntax

`ChestSetDestroyWhenEmpty(chest_id,destroy_when_empty);`

**Returns** undefined.

| **Argument**        | **Type** | **Description**                |
|-----------------------|----------|--------------------------------|
| chest_id              | String   | The chest ID to modify.        |
| destroy_when_empty    | Boolean  | Whether the chest is destroyed |

Sets the name of the chest which is displayed on the UI.

### Example:

```
-- Create a chest
ChestCreate("new_chest")
-- Set the destroy when empty behavior
ChestSetDestroyWhenEmpty("new_chest",true)
```

The above code creates a new chest and then names it.