# ItemConsumableSetEvent

### Syntax

`ItemConsumableSetEvent(item_id, function);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description** |
|---|---|---|
| item_id | String | The name of the item to assign the sprite to. |
| function | Function | The function that is performed when you consume the item. |

Assigns a function to be performed when this item is consumed.

### Example:

```
-- Modify the consumption event of the bandage item
ItemConsumableSetEvent("bandage", func() {
  ShowMessage("I used a bandage!")
})
```

The above code will cause a message to appear when the bandage item is consumed.