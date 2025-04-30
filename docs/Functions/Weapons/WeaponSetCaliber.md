# WeaponSetCaliber

### Syntax

`WeaponSetCaliber(item_id,caliber);`

**Returns** undefined.

| **Argument** | **Type** | **Description** |
|---|---|---|
| item_id | String | A name to use as a reference to the item. |
| caliber | String | The caliber used for this weapon. This can be anything you want. |

You can use this function to modify the caliber used for the weapon.

### Example:

```
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
WeaponSetCaliber("new_weapon","test_caliber")
```

The above code creates a new weapon item, and then sets the caliber. In this case, it's already set to the same value but this is an example, so.