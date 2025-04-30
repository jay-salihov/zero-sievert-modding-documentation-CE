# SpeakerGetIndex

### Syntax

`SpeakerGetIndex(speaker_id);`

**Returns** the index number of the speaker.

| **Argument** | **Type** | **Description** |
|---|---|---|
| speaker_id | String | The ID of the speaker to modify. |

This function can be used to get the speaker index of a speaker.

### Example:

```
SpeakerCreate("test_npc")
let _speaker_index = SpeakerGetIndex("test_npc")
```

This creates a speaker and then gets its speaker index.