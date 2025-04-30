# SpeakerAddHello

### Syntax

`SpeakerAddHello(speaker_id, text);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| speaker_id   | String   | The ID of the speaker to modify.                 |
| text         | String   | The text shown when you first interact with this speaker. |

Allows you to set the dialogue shown when you first talk to a speaker.

### Example:

```
SpeakerCreate("test_npc") SpeakerAddHello("test_npc","Hey there stranger!") 
```

This creates a speaker and then sets the hello message for it.