# QuestCreate

### Syntax

`QuestCreate(quest_id);`

**Returns** undefined, otherwise it will crash.

| **Argument** | **Type** | **Description**                          |
| :----------- | :------- | :--------------------------------------- |
| quest_id     | String   | A name to use as a reference to the quest. |

Create a new quest that can be affected and referred to by its *__quest_id__*.

### Example:

```
-- Create our quests
QuestCreate("kill_quest")
QuestSetName("kill_quest","The Test Quest")
QuestSetText("kill_quest","You'll have to go and kill 1 wolf for me. I have a personal agenda against wolves.")
QuestAddObjective("kill_quest", QuestObjectiveTypeKill( 1, "Wolves", -1,["wolf_brown"], 0, "" ) )
QuestAddReward("kill_quest","pills_anti_rad",1)
```

The above code create a new quest and assign it some dialogue, and then, an objective and reward.