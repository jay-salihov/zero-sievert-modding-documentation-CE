# WeaponCopy

### Syntax

`WeaponCopy(item_id,weapon_id_to_copy);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                                                 |
| :----------- | :------- | :------------------------------------------------------------------------------ |
| item_id      | String   | A name to use as a reference to the item.                                      |
| item_id_to_copy | String   | The item id to copy from. Here's a list of all the [Item IDs](Item IDs) in the game by default. |

Create a new weapon item that can be affected and referred to by its ***item_id*** but the data for this weapon is an exact copy of another item.

It will be a duplicate but not a reference meaning you can use this to create a weapon from another like a template.

### Example:

```
-- Now create a weapon from a copy 
WeaponCopy("new_weapon","glock_17_1")
```

The above code creates a new weapon by making a copy of the **glock_17_1**.