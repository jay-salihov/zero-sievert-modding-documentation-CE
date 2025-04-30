# ItemGrenadeSetThrowMin

### Syntax

`ItemGrenadeSetThrowMin(item_id, distance);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                    |
| :----------- | :------- | :------------------------------------------------- |
| item_id      | String   | The name of the item to adjust.                    |
| distance     | Int      | How far the player can throw a grenade.            |

***ItemGrenadeSetThrowMin and ***ItemGrenadeSetThrowMax*** are used to change the distance the player can throw the selected grenade. The grenade will land at a point in between these distances depending on where the mouse / gamepad crosshair is on the screen.

### Example:

```
ItemGrenadeSetThrowMin("example grenade", 150)
```

The above code will change the grenade *"example grenade"* so it cannot be thrown less than 150 away from the player. If the cursor goes nearer to the player the grenade will still land outside this range.