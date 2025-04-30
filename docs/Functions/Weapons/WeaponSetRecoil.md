# WeaponSetRecoil

### Syntax

`WeaponSetRecoil(item_id,recoil);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                             |
| :----------- | :------- | :---------------------------------------------------------- |
| item_id      | String   | A name to use as a reference to the item.                  |
| recoil       | Real     | The recoil value of the weapon, affects the kickback when firing. |

You can use this function to modify the recoil value of the weapon. This affects the kickback when firing a weapon.

### Example:

```
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
WeaponSetRecoil("new_weapon",50)
```

The above code creates a new weapon item, and then sets the recoil.