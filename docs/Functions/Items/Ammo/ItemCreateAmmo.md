# ItemCreateAmmo

### Syntax

```
ItemCreateAmmo(item_id, caliber="", accuracy=0,damage=0,durability_loss=0.015, effective_range="rifle", number=1, penetration=25, recoil=0 , shell=0);
```

**Returns** undefined.

| **Argument**    | **Type** | **Description**                                                                |
| :-------------- | :------- | :----------------------------------------------------------------------------- |
| item_id         | String   | A name to use as a reference to the item.                                     |
| caliber         | String   | Caliber used. [Calibers](Calibers)                                             |
| accuracy        | Real     | The accuracy bonus provided by this ammo.                                      |
| damage          | Real     | The damage bonus provided by this ammo.                                        |
| durability_loss | Real     | The durability lost by the weapon each shot.                                   |
| effective_range | String   | The effective range of the weapon while using this ammo.                         |
| number          | Int      | The number of bullet per shot.                                                 |
| penetration     | Real     | Penetration value.                                                             |
| recoil          | Real     | The recoil bonus provided by this ammo.                                        |
| shell           | Int      | The color of the shell created.                                                |

Create a new ammo.

**caliber**: use an existing caliber or create a new one. The game will automatically create a new caliber if a custom name is written here.

**effective_range**: use **"{use_weapon}"** to not overwrite the effective range of the weapon while using this ammo. See example

**shell** accept a value from 0 to 9. See the colors here:  
“Pasted image 20250318105919.png” could not be found.

### Example:

```
-- Add an ammo to an already existing caliber
ItemCreateAmmo("ammo_545x39_pp", "a545x39", 0, 0, 0.05, "{use_weapon}", 1, 35, 5,4)

-- Create two new ammos for a new caliber
ItemCreateAmmo("new_ammo_standard", "new_caliber", 0, 0, 0.05, "{use_weapon}", 1, 20, 0,9)
ItemCreateAmmo("new_ammo_AP", "new_caliber", -5, -5, 0.10, "sniper", 1, 50, 10,9)
```

In the last example, using "sniper" means that no matter the weapon we are using, while using this ammunition the effective range is gonna be the same of the sniper one