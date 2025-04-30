# WeaponSetErgonomics

### Syntax

`WeaponSetErgonomics(item_id,ergonomics);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                   |
| :----------- | :------- | :------------------------------------------------ |
| item_id      | String   | A name to use as a reference to the item.        |
| ergonomics   | Real     | The ergonomics value of the weapon, affects handling. |

You can use this function to modify the ergonomics value of the weapon. This affects the mouse tracking and recoil of the weapon.

### Example:

```
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
WeaponSetErgonomics("new_weapon",50)
```

The above code creates a new weapon item, and then sets the ergonomics value.