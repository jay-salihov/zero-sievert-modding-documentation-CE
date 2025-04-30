# QuestAddObjective

### Syntax

`QuestAddObjective(quest_id, objective_data);`

**Returns** undefined, otherwise it will crash.

| **Argument**   | **Type** | **Description**                                                                                                |
| :------------- | :------- | :------------------------------------------------------------------------------------------------------------- |
| quest_id       | String   | A name to use as a reference to the ques                                                                      |
| objective_data |          | Objective data to build objective data you will need to use one of the QuestObjectiveType* functions. See examples here: ??? |

With this function you can add an objective to a quest. You can add one objective at a time.

### Example:

```lua
-- Create our quests
QuestCreate("kill_quest")
-- Set the quest name
QuestAddObjective("kill_quest", QuestObjectiveTypeKill( 1, "Wolves", -1,["wolf_brown"], 0, "" ) )
```

The above code creates a new quest and adds an objective to it. The objective is to kill 1 wolf.