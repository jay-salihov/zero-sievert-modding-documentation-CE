# WeaponSetReloadTime

### Syntax

`WeaponSetReloadTime(item_id,reload_time);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                      |
| :----------- | :------- | :--------------------------------------------------- |
| item_id      | String   | A name to use as a reference to the item.           |
| reload_time  | Real     | The reload time affects how long it takes to reload the weapon. |

You can use this function to modify the reload time of the weapon.

### Example:

```
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
WeaponSetReloadTime("new_weapon",90)
```

The above code creates a new weapon item, and then sets the reload time.