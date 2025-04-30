# ItemGrenadeSetThrowMax

### Syntax

`ItemGrenadeSetThrowMax(item_id, distance);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
| ------------ | -------- | --------------------------------------------- |
| item_id      | String   | The name of the item to adjust.               |
| distance     | Int      | How far the player can throw a grenade.       |

***ItemGrenadeSetThrowMin and*** *ItemGrenadeSetThrowMax*** are used to change the distance the player can throw the selected grenade. The grenade will land at a point in between these distances depending on where the mouse / gamepad crosshair is on the screen.

### Example:

```
ItemGrenadeSetThrowMax("example grenade", 300) 
```

The above code will change the grenade *"example grenade"* so the maximum distance it can be thrown is 300. If the cursor goes outside this range the grenade will still land this distance away from the player.