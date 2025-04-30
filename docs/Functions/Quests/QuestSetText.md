# QuestSetText

### Syntax

`QuestSetText(quest_id, quest_text);`

**Returns** undefined, otherwise it will crash.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| quest_id     | String   | A name to use as a reference to the quest.      |
| quest_text   | String   | The dialogue text that is shown in relation to the quest. |

Sets the dialogue text for the quest. This is not the same as the objective text.

### Example:

```
-- Create our quests
QuestCreate("kill_quest")
-- Set the quest name
QuestSetText("kill_quest","You'll have to go and kill 1 wolf for me.")
```

The above code creates a new quest and sets its dialogue text.