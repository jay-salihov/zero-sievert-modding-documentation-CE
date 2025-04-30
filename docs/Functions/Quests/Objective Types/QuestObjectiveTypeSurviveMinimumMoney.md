# QuestObjectiveTypeSurviveMinimumMoney

### Syntax

`QuestObjectiveTypeSurviveMinimumMoney(map, amount_max, amount_money, marker_radius, text);`

**Returns** undefined, otherwise it will crash.

| **Argument** | **Type** | **Description** |
| --- | --- | --- |
| map | Real | If you want a specific map for this objective you can use one of the maps listed on the [Map Names](Map Names) page, or use a map_id from a custom map. If you don't want to specify a map, use -1 instead. |
| amount_max | Real | The amount of times the player has to survive. |
| amount_money | Real | The amount of money needed to complete the objective. |
| marker_radius | Real | The size of the marker shown on the map for this objective. |
| text | String | The text description for this objective, you can leave it as "" if you want to have it auto-generate a description. |

Generates a money-goal survival objective to be used with a quest. This function should used to provide an objective to the function [QuestAddObjective](QuestAddObjective).

### Example:

```
-- Create our quests
QuestCreate("survivemoney_quest")

-- Set the quest name
QuestAddObjective("survivemoney_quest", QuestObjectiveTypeSurviveMinimumMoney( MAP_forest, 1, 100, 0, "" ) )
```

The above code creates a new quest and adds an objective to it. The objective is to survive the forest map once with $100.