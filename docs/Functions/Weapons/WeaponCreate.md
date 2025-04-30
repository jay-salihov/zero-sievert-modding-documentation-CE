# WeaponCreate

### Syntax

`WeaponCreate(item_id,weapon_type,moddable,ammo_item_id,ammo_caliber,attachment_array);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                                                                                                                                              |
| :----------- | :------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| item_id      | String   | A name to use as a reference to the item.                                                                                                                                    |
| weapon_type  | String   | Defines the weapon type, used for glancing damage and effective range. See the [Weapon Types](Weapon Types) for a list of available options.                                  |
| moddable     | Boolean  | Whether or not a weapon can have mods attached/detached.                                                                                                                     |
| ammo_item_id | String   | The item_id of the ammo to be used for this weapon.                                                                                                                            |
| ammo_caliber | String   | The caliber of ammo to be used for this weapon.                                                                                                                               |
| attachment_array | Array   | An array of attachment slots and positions. See the example provided down below.                                                                                                                               |

Create a new weapon item that can be affected and referred to by its ***item_id***.

If you have a handguard built into the weapon that is not removable, you can use the *attachment_array* for this weapon and instead of attaching to your handguard, the attachments will attach directly to the weapon.

### Example:

```lua
-- Load our item sprite
SpriteLoad("test_weapon","test_weapon.png",1,0,0,0);
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
-- Now assign our "test_weapon" sprite to our new weapon, "new _weapon"
ItemSetSpriteInventory("new_weapon",SpriteGet("test_weapon"))
ItemSetSpriteIngame("new_weapon",SpriteGet("test_weapon"))
```

The above code loads a new sprite, creates a new weapon item, and then assigns the new sprite to the new weapon item.