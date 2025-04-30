# SpeakerAddDialogueChoice

### Syntax

`SpeakerAddDialogueChoice(speaker_id, dialogue_type, text);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                    |
| :----------- | :------- | :------------------------------------------------- |
| speaker_id   | String   | The ID of the speaker to modify.                   |
| dialogue_type| String   | The type of dialogue to use. See [Speaker Dialogue Types](Speaker_Dialogue_Types.md) for options. |
| text         | String   | The text shown for this dialogue choice.           |

Adds a new dialogue choice to a speaker.

### Example:

```
SpeakerCreate("test_npc")
SpeakerAddDialogueChoice("test_npc",DIALOGUE_TYPE_back,"Ok bye nerd!")
```

This creates a speaker and then adds a dialogue choice to the speaker.