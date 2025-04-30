# QuestObjectiveTypeCollect

### Syntax

`QuestObjectiveTypeCollect(item, amount_max, marker_radius, text);`

**Returns** undefined, otherwise it will crash.

| **Argument** | **Type** | **Description**                                                      |
| :----------- | :------- | :------------------------------------------------------------------- |
| item         | String   | The item_id of the item to collect.                                |
| amount_max   | Real     | The quantity of the item required for objective completion.          |
| marker_radius| Real     | The size of the marker shown on the map for this objective.         |
| text         | String   | The text description for this objective, you can leave it as "" if you want to have it auto-generate a description. |

Generates a collect objective to be used with a quest. This function should used to provide an objective to the function [QuestAddObjective](QuestAddObjective).

### Example:

```
-- Create our quests
QuestCreate("collect_quest")

-- Set the quest name
QuestAddObjective("collect_quest", QuestObjectiveTypeCollect( "bandage", 1, 0, "" ) )
```

The above code creates a new quest and adds an objective to it. The objective is to collect 1 bandage.