# QuestSetName

### Syntax

`QuestSetName(quest_id, quest_name);`

**Returns** undefined, otherwise it will crash.

| **Argument** | **Type** | **Description**                       |
| :----------- | :------- | :------------------------------------ |
| quest_id     | String   | A name to use as a reference to the quest. |
| quest_name   | String   | The name to be displayed for the quest. |

Sets the displayed name for a quest.

### Example:

```
-- Create our quests
QuestCreate("kill_quest")
-- Set the quest name
QuestSetName("kill_quest","The Test Quest")
```

The above code creates a new quest and sets its name.