# ItemGrenadeSetFuseTime

### Syntax

`ItemGrenadeSetFuseTime(item_id, duration);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                     |
|--------------|----------|-----------------------------------------------------|
| item_id      | String   | The name of the item to adjust.                     |
| duration     | Int      | Number of frames until detonation.                  |

This changes how long after the player presses throw it will take for the grenade to explode. This time also includes the time the grenade is in the air. The grenade is in the air for about 70 frames so if you want the grenade to explode the moment it hits the floor this value can be set to around 70. If you want to make an airburst grenade a value like 26 can be set. 

The duration is done in frames and the game runs at 60 frames per second. Because of this setting the duration to 60 will make it last for 1 second. 120 is two second etc. 

### Example:

```
ItemGrenadeSetFuseTime("example grenade", 120) 
```

The above code will change the grenade *"example grenade"* so that two seconds after the player presses to throw the grenade will detonate. 