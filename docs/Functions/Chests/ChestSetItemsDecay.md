# ChestSetItemsDecay

### Syntax

`ChestSetItemsDecay(chest_id,decay_items);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| chest_id     | String   | The chest ID to modify.                       |
| decay_items  | Boolean  | Whether or not the items in this chest will decay. |

Used to determine whether or not items in the chest will decay.

### Example:

```
-- Create a chest
ChestCreate("new_chest")
-- Set items to decay
ChestSetItemsDecay("new_chest",true)
```

The above code creates a new chest and then sets items in the chest to decay.