# SoundGet

### Syntax

`SoundGet(sound_name);`

**Returns** the sound if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                   |
| :----------- | :------- | :------------------------------ |
| sound_name   | String   | The name of the sound to get. |

Gets a sound that was previously added with [SoundLoad](SoundLoad). You will need to do this when assigning sounds to weapons or items.

### Example:

```
-- Load our sound
SoundLoad("test_sound","test_sound.ogg");

-- Now play the sound
SoundPlay("test_sound");
```

The above code loads a new sound and then plays it.