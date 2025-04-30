# ItemCreate

### Syntax

`ItemCreate(item_id, category="none");`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                          |
| :----------- | :------- | :------------------------------------------------------- |
| item_id      | String   | A name to use as a reference to the item.               |
| category     | String   | Defines the type of item this is, see the [Item Categories](Item Categories) page. |

Create a new item that can be affected and referred to by its ***item_id***. This is specifically a generic function to provide a generic item. For example, while weapons are still items, you should use ***WeaponCreate()*** when creating weapons.

### Example:

```
-- Now create an item ItemCreate("new_item","none") 
```

The above code creates a new item.