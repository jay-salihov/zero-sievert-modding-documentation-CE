# WeaponSetWeaponType

### Syntax

`WeaponSetWeaponType(item_id,weapon_type);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                                                                                 |
| :----------- | :------- | :-------------------------------------------------------------------------------------------------------------- |
| item_id      | String   | A name to use as a reference to the item.                                                                      |
| weapon_type  | String   | The weapon type that the weapon should use, see [Weapon Types](Weapon Types) for a list of available options. |

You can use this function to modify the firing mode of a weapon.

### Example:

```
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
WeaponSetWeaponType("new_weapon","rifle")
```

The above code creates a new weapon item, and then sets the firing mode for the weapon.