# ItemInjectorSetDuration

### Syntax

`ItemInjectorSetDuration(item_id, duration);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
|--------------|----------|-----------------------------------------------|
| item_id      | String   | The name of the item to update.               |
| duration     | Real     | Number of frames effects last for.            |

Once this injector is used changes how long the effects last for. This is in number of frames, the game runs at 60 frames per second so 600 would be 10 seconds.