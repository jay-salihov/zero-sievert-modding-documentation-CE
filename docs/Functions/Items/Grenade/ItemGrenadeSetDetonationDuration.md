# ItemGrenadeSetDetonationDuration

### Syntax

`ItemGrenadeSetDetonationDuration(item_id, duration);`

**Returns** “*__true__*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                   | Default |
| :----------- | :------- | :------------------------------ | :------ |
| item_id      | String   | The name of the item to adjust. |         |
| duration     | Int      | Duration in frames (at 60fps)   | 0       |

After the grenade explodes it will repeatedly do damage for this number of frames.

If this is set to 0 it will only trigger the damage effect once. **Please note:** Because of this if *duration* is set to 1 it will do double damage.

It can be used to give the grenade a lingering effect though.

The duration is done in frames and the game runs at 60 frames per second. Because of this setting the duration to 60 will make it last for 1 second. 120 is two second etc.