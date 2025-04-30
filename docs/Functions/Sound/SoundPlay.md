# SoundPlay

### Syntax

`SoundPlay(sound_name, loop=false, gain=1, pitch=1);`

**Returns** the *sound_id* if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                                                  |
|--------------|----------|----------------------------------------------------------------------------------|
| sound_name   | String   | The name of the sound to get.                                                    |
| loop         | Boolean  | Whether or not the sound should loop.                                            |
| gain         | Real     | The volume of the sound from 0 - 1. The default is 1. A value of 0 would be muted. |
| pitch        | Real     | The pitch of the sound from. The default is 1. This is a multiplier so a value of 2 doubles the pitch. |

Plays a sound that was previously loaded with [SoundLoad](SoundLoad).

### Example:

```
-- Load our sound
SoundLoad("test_sound","test_sound.ogg");

-- Now play the sound
SoundPlay("test_sound");
```

The above code loads a new sound and then plays it.