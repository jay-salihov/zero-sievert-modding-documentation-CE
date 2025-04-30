# ItemGrenadeSetDamageMin

### Syntax

`ItemGrenadeSetDamageMin(item_id, animation);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| item_id      | String   | The name of the item to adjust.                  |
| damage       | Float    | The damage done inside the max damage radius. |

When calculating the damage the grenade does this will be the minimum amount of damage taken at the edge of ***RadiusMinDamage*** .

<span><img/></span>

### Example:

```
ItemGrenadeSetDamageMin("example grenade id", 10)
```

The above code will change set the grenade called *"example grenade id"* to do 10 damage at the very edge of ***RadiusMinDamage***.

For example if **RadiusMaxDamage** is 100 and ***RadiusMinDamage*** is 50 someone standing halfway between them will take 75 damage.