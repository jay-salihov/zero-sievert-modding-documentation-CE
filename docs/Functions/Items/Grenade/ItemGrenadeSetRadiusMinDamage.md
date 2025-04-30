# ItemGrenadeSetRadiusMinDamage

### Syntax

`ItemGrenadeSetRadiusMinDamage(item_id, distance);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                    |
| :----------- | :------- | :------------------------------------------------- |
| item_id      | String   | The name of the item to adjust.                    |
| distance     | Float    | Distance from grenade centre to impact characters. |

When a grenade detonate, this is used to change the radius of the effect. There are two settings the radius of the min damage and the radius of the max damage.

<span><img/></span>

When someone takes damage from this grenade if they are right on the edge of RadiusMinDamage they will take ***DamageMin*** damage.

To help gauge size in the image above **RadiusMaxSize** is set to *23* and **RadiusMinSize** is set to *54*.

### Example:

```
ItemGrenadeSetRadiusMinDamage("example grenade", 50) 
```

The above code will change the grenade *"example grenade"* the area that max damage is does is 50 radius .