# ItemGrenadeSetDamageMax

### Syntax

`ItemGrenadeSetDamageMax(item_id, animation);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                     |
| :----------- | :------- | :------------------------------------ |
| item_id      | String   | The name of the item to adjust.       |
| damage       | Float    | The damage done inside the max damage radius. |

When calculating the damage this grenade does anyone inside ***RadiusMaxDamage*** will take ***DamageMax***. If the effected enemy is between ***RadiusMaxDamage*** and ***RadiusMinDamage*** a value between the ***DamageMax*** and ***DamageMin*** will be used. 

<span><img/></span>

### Example:

```
ItemGrenadeSetDamageMax("example grenade id", 120) 
```

The above code will change set the grenade called *"example grenade id"* to do 120 damage inside the ***RadiusMaxDamage*** red zone and between the min and max zones it will be some value between ***RadiusMaxDamage*** and ***RadiusMinDamage***.

For example if **RadiusMaxDamage** is 100 and ***RadiusMinDamage*** is 50 someone standing halfway between them will take 75 damage.