# ChestSetSoundType

### Syntax

`ChestSetSoundType(chest_id,sound_type);`

**Returns** undefined.

| **Argument** | **Type** | **Description** |
|---|---|---|
| chest_id | String | The chest ID to modify. |
| sound_type | String | The sound type to use. Use one of the values from the list below. |

Sets the sound effect used when you interact with the chest.

| Sound Types |
|---|
| "box" |
| "meat" |
| "body" |
| "bag" |
| "cabinet" |
| "cash_register" |
| "cristallo" |
| "safe" |

### Example:

```
-- Create a chest
ChestCreate("new_chest")
-- Set the chest sound
ChestSetSoundType("new_chest","safe")
```

The above code creates a new chest and then sets the chest sound type.