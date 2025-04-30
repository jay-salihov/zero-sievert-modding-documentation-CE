# SpeakerAddQuest

### Syntax

`SpeakerAddQuest(speaker_id, quest_id);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                       |
| :----------- | :------- | :------------------------------------ |
| speaker_id   | String   | The ID of the speaker to modify.      |
| quest_id     | String   | The ID for the quest you would like to add. |

This can be used to add a new quest to a speaker.

### Example:

```
SpeakerCreate("test_npc") SpeakerSetMoves("test_npc",true)
```

This creates a speaker and then adds a quest.