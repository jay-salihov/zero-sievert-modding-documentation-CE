# WeaponSetScript

### Syntax

`WeaponSetScript(item_id,event_id,function);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                                                                                                              |
| :----------- | :------- | :------------------------------------------------------------------------------------------------------------------------------------------- |
| item_id      | String   | A name to use as a reference to the item.                                                                                                   |
| event_id     | String   | The ID for the event that a function should be assigned to.                                                                                  |
| function     | Function | A function provided that will run in the context of either the weapon or the bullet depending on the event. See the event IDs that are available here: [Weapon Script Events](Weapon Script Events) |

You can use this to assign custom functions to be performed during specific events for a weapon.

### Example:

```
-- Now create a weapon
WeaponCreate("new_weapon","rifle",false,"test_ammo","test_caliber")
WeaponSetScript("new_weapon","weapon_fire",func(_inst)
  {
    _inst.x += LengthDirX(5,_inst.weapon_pointing_direction + 180);
    _inst.y += LengthDirY(5,_inst.weapon_pointing_direction + 180);
  })
```

The above code creates a new weapon item, and then creates a function that is assigned to the "weapon_fire" event.