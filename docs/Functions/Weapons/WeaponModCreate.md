# WeaponModCreate

### Syntax

`WeaponModCreate(item_id, mod_type="grip", accuracy=0,damage=0, ergonomics=0, recoil=0, reload_speed=0, scope_optic=false, compatible_weapons=[], attachment_array=[]);`

**Returns** undefined.

| **Argument**        | **Type** | **Description**                                                                                                                                                                                                                                                                                                                                               |
| :------------------ | :------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| item_id             | String   | A name to use as a reference to the item.                                                                                                                                                                                                                                                                                                                    |
| mod_type            | String   | Defines the type of weapon mod this item is. See [Weapon Mod Types](Weapon Mod Types) for a list of available mod types.                                                                                                                                                                                                                                       |
| accuracy            | Real     | The accuracy bonus provided by this mod.                                                                                                                                                                                                                                                                                                                     |
| damage              | Real     | The damage bonus provided by this mod.                                                                                                                                                                                                                                                                                                                       |
| ergonomics          | Real     | The ergonomics bonus provided by this mod.                                                                                                                                                                                                                                                                                                                    |
| recoil              | Real     | The recoil bonus provided by this mod.                                                                                                                                                                                                                                                                                                                       |
| reload_speed        | Real     | The reload speed bonus provided by this mod.                                                                                                                                                                                                                                                                                                                   |
| scope_optic         | Boolean  | Whether or not this is an optic scope.                                                                                                                                                                                                                                                                                                                       |
| compatible_weapons  | Array    | An array of all the item id's that this mod is compatible with.                                                                                                                                                                                                                                                                                              |
| attachment_array | Array    | An array of attachment slots and positions. See the example provided down below.                                                                                                                                                                                                                                                                                              |

Create a new weapon mod item that can be affected and referred to by its ***item_id***. See the [Weapon Mod Types](Weapon Mod Types) page for all available weapon mods.

An important note, foregrips can only be attached to "att_1" on weapons.
If you want your attachments to be compatible with all weapons, put "[]" in *compatible_weapons* slot. See example

### Example:

```
WeaponModCreate("mod_test_magazine", "magazine", 0, 0, 0, 0, 0, false, ["test_weapon"])
WeaponModSetWeaponModData("test_weapon", "magazine", "mod_test_magazine", true, 0, 0)
WeaponModCreate("handguard_test","handguard",0,0,0,0,0,false,["test_weapon"],[["att_1",5,5]])
WeaponSetMagazineModCapacity("mod_test_magazine", 20)
-- Attachement compatible with all weapons
WeaponModCreate("scope_test","scope",0,0,0,0,0,true,[])
```

The above code creates a weapon mod, assigns that weapon mod to be the default magazine mod for "test_weapon", and then sets the mod's magazine capacity to 20.