# ItemWeaponRepairCreate

### Syntax

`ItemWeaponRepairCreate(item_id, high, weapon_class);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                  | **Default** |
| :----------- | :------- | :----------------------------------------------- | :---------- |
| item_id      | String   | The name that can be used to refer to it in the future. |             |
| high         | true/false | High or low recovery.                            | true        |
| weapon_class | Array    | Which weapon calibres this item can be used on. | []          |

Create a new repair item that can be affected and referred to by its *<strong>item_id</strong>*.

Allowed values for weapon class:

| Values:    |
| :---------- |
| "a9x18"     |
| "a9x19"     |
| "a57x28"    |
| "a12x70"    |
| "a357magnum" |
| "a762x25"    |
| "a762x51"    |
| "a762x54r"   |
| "a127x55"   |
| "a9x39"     |
| "a545x39"    |
| "a556x45"    |
| "a762x39"    |
| "a45"       |

### Example:

```
ItemWeaponRepairCreate("Dave Weapon Repair",false,["a9x18","a9x39","a357magnum","a45"])
SpriteLoad("Dave Weapon Repair","test_item.png",1,0,0,0)
ItemSetSpriteInventory("Dave Weapon Repair","test_item")
ItemSetSpriteIngame("Dave Weapon Repair","test_item")
ItemSetName("Dave Weapon Repair", "Daves Weapon Repair Item")
```

The above code will create a new repair item that can be spawned in the future and referred to as: "Dave Weapon Repair". It will have the icon "test_item.png" and can only be used on these calibre weapons: "a9x18","a9x39","a357magnum","a45". It will do a low amount of repair.