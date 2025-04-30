# ItemGrenadeCreate

### Syntax

`ItemGrenadeCreate(item_id);`

**Returns** “* **true** *“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                       |
| :----------- | :------- | :---------------------------------------------------- |
| item_id      | String   | The name that can be used to refer to it in the future. |

This function creates a new grenade that can be affected and referred to by its * **item_id** *. Backpacks can be equipped by the player and thrown like a weapon.

### Example:

```
ItemGrenadeCreate("Example Grenade");
SpriteLoad("Grenade Image","test_item.png",1,0,0,0)
ItemSetSpriteInventory("Example Grenade","Grenade Image")
ItemSetSpriteIngame("Example Grenade","Grenade Image")
ItemSetName("Example Grenade", "Daves Big Grenade")
ItemGrenadeSetAnimation("Example Grenade","s_arms_grenade_f1")
ItemGrenadeSetDamageMax("Example Grenade",150)
ItemGrenadeSetDamageMin("Example Grenade",50)
ItemGrenadeSetDetonationDuration("Example Grenade",0)
ItemGrenadeSetDetonationType("Example Grenade","GRENADE_detonation_explosion")
ItemGrenadeSetFuseTime("Example Grenade",120)
ItemGrenadeSetRadiusMaxDamage("Example Grenade",16)
ItemGrenadeSetRadiusMinDamage("Example Grenade",28)
ItemGrenadeSetRadiusRadiusEffect("Example Grenade",48)
ItemGrenadeSetThrowMax("Example Grenade",100)
ItemGrenadeSetThrowMin("Example Grenade",50)
ItemGrenadeSetThrowType("Example Grenade","GRENADE_throw_bounce")
```

The above code will create a new grenade item that can be spawned in the future and referred to as: "Example Grenade". It will have the inventory icon "test_item.png" and the name "Daves Big Grenade". This grenade can be equipped into quick slots and thrown.

### Default values that can be updated:

| Key:              | Value:                        |
| :---------------- | :---------------------------- |
| weight            | 0                             |
| carry weight      | 0.5                           |
| value             | 5000                          |
| animation         | "s_arms_grenade_rgd"          |
| throw_min         | 48                            |
| throw_max         | 210                           |
| fuse_time         | 120                           |
| throw_type        | "GRENADE_throw_bounce"        |
| damage_max        | 150                           |
| damage_min        | 50                            |
| detonation_type   | "GRENADE_detonation_explosion" |
| detonation_duration | 0                             |
| radius_max_damage | 32                            |
| radius_min_damage | 52                            |
| radius_effect     | 64                            |