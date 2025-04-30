# QuestObjectiveTypeKill

### Syntax

`QuestObjectiveTypeKill(amount_max, faction,map, array_kill, marker_radius, text);`

**Returns** undefined, otherwise it will crash.

| **Argument**   | **Type** | **Description**                                                                                                                                                                                                                                      |
| :------------- | :------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| amount_max     | Real     | Amount of the enemy to kill.                                                                                                                                                                                                                        |
| faction        | String   | The faction name for the enemy to kill. See [Faction Names](Faction Names), you can make your own faction names for enemies such as Wolves.                                                                                                          |
| map            | Real     | If you want a specific map for this objective you can use one of the maps listed on the [Map Names](Map Names) page, or use a map_id from a custom map. If you don't want to specify a map, use -1 instead.                                        |
| array_kill     | Array    | An array of enemies to be killed. See [Enemy Names](Enemy Names) for a list of enemy names that can be used without adding your own.                                                                                                                 |
| marker_radius  | Real     | The size of the marker shown on the map for this objective.                                                                                                                                                                                          |
| text           | String   | The text description for this objective, you can leave it as "" if you want to have it auto-generate a description.                                                                                                                                  |

Generates a kill objective to be used with a quest. This function should used to provide an objective to the function [QuestAddObjective](QuestAddObjective).

### Example:

```lua
-- Create our quests 
QuestCreate("kill_quest") 
-- Set the quest name 
QuestAddObjective("kill_quest", QuestObjectiveTypeKill( 1, "Wolves", -1,["wolf_brown"], 0, "" ) )
```

The above code creates a new quest and adds an objective to it. The objective is to kill 1 wolf.