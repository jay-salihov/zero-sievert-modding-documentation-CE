# SoundPlayAt

### Syntax

`SoundPlayAt(sound_name, falloff_max_dist, loop=false, gain=1, pitch=1);`

**Returns** the *sound_id* if successful, otherwise it will crash.

| **Argument**        | **Type** | **Description**                                                 |
| ------------------- | -------- | --------------------------------------------------------------- |
| sound_name          | String   | The name of the sound to get.                                 |
| x                   | Real     | The x position to play the sound at.                          |
| y                   | Real     | The y position to play the sound at.                          |
| falloff_max_dist    | Real     | The max distance that you can hear the sound from.            |
| loop                | Boolean  | Whether or not the sound should loop.                         |
| gain                | Real     | The volume of the sound from 0 - 1. The default is 1. A value of 0 would be muted. |
| pitch               | Real     | The pitch of the sound from. The default is 1. This is a multiplier so a value of 2 doubles the pitch. |

Plays a sound that was previously loaded with [SoundLoad](SoundLoad).

### Example:

```lua
-- Load our sound
SoundLoad("test_sound","test_sound.ogg");

-- Now play the sound
SoundPlay("test_sound");
```

The above code loads a new sound and then plays it.