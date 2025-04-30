# WeaponSetFireMode

### Syntax

`WeaponSetFireMode(item_id,fire_mode);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                                                |
| :----------- | :------- | :----------------------------------------------------------------------------- |
| item_id      | String   | A name to use as a reference to the item.                                     |
| fire_mode    | String   | The fire mode that the weapon should use, see [Weapon Firing Modes](Weapon Firing Modes) for a list of available options. |

You can use this function to modify the firing mode of a weapon.

### Example:

```
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
WeaponSetFiringMode("new_weapon","semi_automatic")
```

The above code creates a new weapon item, and then sets the firing mode for the weapon.