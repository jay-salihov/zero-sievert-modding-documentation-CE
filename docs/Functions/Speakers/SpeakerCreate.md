# SpeakerCreate

### Syntax

`SpeakerCreate(speaker_id);`

**Returns** the "* **struct** *" that is created for the speaker.

| **Argument** | **Type** | **Description**                       |
| :----------- | :------- | :------------------------------------ |
| speaker_id   | String   | A name to reference the speaker.      |

Creates a new speaker that can be used with NPCs. Speakers contain dialogue choices, sprites, and a few other elements. A speaker can be reused for multiple NPCs in the same area which is helpful for enemy NPCs that don’t really use dialogue.

### Example:

```
-- Create our speaker
SpeakerCreate("test_npc")
SpeakerAddDialogueChoice("test_npc",DIALOGUE_TYPE_back,"See ya!")
SpeakerAddDialogueChoice("test_npc",DIALOGUE_TYPE_question,"I have some questions.")
SpeakerAddQuestion("test_npc","Are you an NPC?","Yes, yes I am."

-- Now create an NPC that uses our new speaker
NpcSpawn("test_npc",100,100)
```

This creates a speaker and then spawn an NPC that uses that speaker data.