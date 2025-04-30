# WeaponSetAmmo

### Syntax

`WeaponSetAmmo(item_id,ammo_item_id);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| item_id      | String   | A name to use as a reference to the item.       |
| ammo_item_id | String   | The ammo item that is used for this weapon. |

You can use this function to modify the ammo item used for the weapon.

### Example:

```
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
WeaponSetAmmo("new_weapon","test_ammo")
```

The above code creates a new weapon item, and then sets the ammo item.