# ItemArmorRepairCreate

### Syntax

`ItemArmorRepairCreate(item_id, high, armour_class_0, armour_class_1, armour_class_2, armour_class_3, armour_class_4, armour_class_5, armour_class_6);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description** | **Default** |
|---|---|---|---|
| item_id | String | The name that can be used to refer to it in the future. |  |
| high | true/false | High or low recovery. | true |
| armor_class_0 | true/false | Can this item be used on armour class 0 items. | true |
| armor_class_1 | true/false | Can this item be used on armour class 1 items. | true |
| armor_class_2 | true/false | Can this item be used on armour class 2 items. | true |
| armor_class_3 | true/false | Can this item be used on armour class 3 items. | true |
| armor_class_4 | true/false | Can this item be used on armour class 4 items. | true |
| armor_class_5 | true/false | Can this item be used on armour class 5 items. | true |
| armor_class_6 | true/false | Can this item be used on armour class 6 items. | true |

Create a new repair item that can be affected and referred to by its *<strong>item_id</strong>*. 

Armour class can be used to change which armours this repair kit can be used on. Generally armour with a higher class is better. 

Note: *ItemArmourRepairCreate() also works with the correct spelling.*

### Example:

```
ItemArmorRepairCreate("Dave Repair Armour",false,true,true,true,false,false,false,false)
SpriteLoad("Dave Repair Armour","test_item.png",1,0,0,0)
ItemSetSpriteInventory("Dave Repair Armour","test_item")
ItemSetSpriteIngame("Dave Repair Armour","test_item")
ItemSetName("Dave Repair Armour", "Daves Armour Repair Item")
```

The above code will create a new repair item that can be spawned in the future and referred to as: "Dave Repair Armour". It will have the icon "test_item.png" and can be used to repair armours of class 0,1,2. The repair amount will be low.