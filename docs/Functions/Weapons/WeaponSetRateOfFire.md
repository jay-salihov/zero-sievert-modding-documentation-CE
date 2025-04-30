# WeaponSetRateOfFire

### Syntax

`WeaponSetRateOfFire(item_id,rate_of_fire);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| item_id      | String   | A name to use as a reference to the item.    |
| rate_of_fire | Real     | The rate of fire used for this weapon.        |

You can use this function to modify the rate of fire used for the weapon.

### Example:

```
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
WeaponSetRateOfFire("new_weapon",3)
```

The above code creates a new weapon item, and then sets the rate of fire.