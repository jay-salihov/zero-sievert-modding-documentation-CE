# NpcSetSpeaker

### Syntax

`NpcSetSpeaker(npc_id,speaker_id);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| npc_id       | String   | The NPC ID that should be used.                 |
| speaker_id   | String   | The Speaker ID that should be used by this NPC. |

Assigns a previously created speaker to an NPC.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Assign our speaker
NpcSetSpeaker("test_npc","test_speaker")
```

The above code will create a NPC and then assign it a speaker to use.