# WeaponSetReloadType

### Syntax

`WeaponSetReloadType(item_id,reload_type);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                                                 |
| :----------- | :------- | :------------------------------------------------------------------------------ |
| item_id      | String   | A name to use as a reference to the item.                                      |
| reload_type  | String   | The reload type that the weapon should use, see [Weapon Reload Types](Weapon Reload Types) for a list of available options. |

You can use this function to modify the firing mode of a weapon.

### Example:

```
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
WeaponSetFiringMode("new_weapon","semi_automatic")
```

The above code creates a new weapon item, and then sets the firing mode for the weapon.