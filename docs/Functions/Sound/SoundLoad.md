# SoundLoad

### Syntax

`SoundLoad(sound_name, file_name);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| sound_name   | String   | A name to use as a reference to the sound.      |
| file_name    | String   | The name (a string file path) of the file to add. |

Loads an external sprite into the game to be used later with the “*sound_name*” provided. The **ONLY** filetype supported are **\*.ogg**.

### Example:

```
-- Load our sound
SoundLoad("test_sound","test_sound.ogg");

-- Now play the sound
SoundPlay("test_sound");
```

The above code loads a new sound and then plays it.