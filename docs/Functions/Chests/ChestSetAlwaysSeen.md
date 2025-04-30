# ChestSetAlwaysSeen

### Syntax

`ChestSetAlwaysSeen(chest_id,always_seen);`

**Returns** undefined.

| **Argument** | **Type** | **Description** |
|---|---|---|
| chest_id | String | The chest ID to modify. |
| always_seen | Boolean | Whether items in this chest are already revealed. |

Sets whether or not items are always seen.

### Example:

```
-- Create a chest
ChestCreate("new_chest")

-- Set whether or not items are revealed
ChestSetAlwaysSeen("new_chest",true)
```

The above code creates a new chest and then sets the items to always be seen.