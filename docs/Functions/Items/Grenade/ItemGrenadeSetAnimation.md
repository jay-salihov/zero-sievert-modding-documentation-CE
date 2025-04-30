# ItemGrenadeSetAnimation

### Syntax

`ItemGrenadeSetAnimation(item_id, animation);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                    |
| :----------- | :------- | :------------------------------------- |
| item_id      | String   | The name of the item to adjust.      |
| animation    | String   | The weight of the item. |

Changes the throw animation when a grenade is used.

#### Built in options:

| Throwing:             |
| :--------------------- |
| s_arms_grenade_f1      |
| s_arms_grenade_flash   |
| s_arms_grenade_mine_pmn|
| s_arms_grenade_rgd     |
| s_arms_grenade_rgn     |
| s_arms_grenade_smoke   |

| All arms:                        |
| :------------------------------- |
| s_arms_drink                     |
| s_arms_drink_cola                |
| s_arms_drink_juice               |
| s_arms_eat                       |
| s_arms_eat_can                   |
| s_arms_eat_chocolate             |
| s_arms_eat_meat                  |
| s_arms_eat_mre                   |
| s_arms_grenade_christmas         |
| s_arms_guitar                    |
| s_arms_med_bandage               |
| s_arms_med_bandage_sterilizzata  |
| s_arms_med_long                  |
| s_arms_med_wound_1               |
| s_arms_med1                      |
| s_arms_scientist_working         |
| s_arms_smoke                     |
| s_arms                           |

### Example:

```
ItemGrenadeSetAnimation("example grenade id", "s_arms_grenade_smoke") 
```

The above code will change the throwing animation when a grenade is used from *s_arms_grenade_rgd* to *s_arms_grenade_smoke*