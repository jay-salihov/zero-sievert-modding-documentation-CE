# Speaker Dialogue Types

When creating dialogue for a speaker with the function `SpeakerAddDialogueChoice`, you’ll need to use a dialogue type as one of the arguments. There are a few types of dialogue that you can use which are listed and explained here.

| **Macro**              | **Description**                                                              |
| ---------------------- | ---------------------------------------------------------------------------- |
| **DIALOGUE_TYPE_back**       | When selected by the player this closes the current conversation.           |
| **DIALOGUE_TYPE_question**   | Opens dialogue into a question answer format that is added to with `SpeakerAddQuestion` |
| **DIALOGUE_TYPE_task**       | Opens dialogue that will list the currently available quests that the speaker has.         |
| **DIALOGUE_TYPE_trade**      | Opens the trading menu with an NPC. Used by all traders.                    |
| **DIALOGUE_TYPE_repair_armor** | Opens the armor repair menu with an NPC. Used by the doctor.             |
| **DIALOGUE_TYPE_heal**       | Opens the healing menu with an NPC. Used by the doctor.                    |
| **DIALOGUE_TYPE_choose_map** | Opens the map selection screen. Used by the conductor.                     |