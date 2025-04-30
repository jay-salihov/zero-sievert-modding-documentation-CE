# QuestAddReward

### Syntax

```
QuestAddReward(quest_id, reward_item, reward_item_quantity);
```

**Returns** undefined, otherwise it will crash.

| **Argument**        | **Type** | **Description**                                     |
| ------------------- | -------- | --------------------------------------------------- |
| quest_id            | String   | A name to use as a reference to the quest.          |
| reward_item         | String   | An item that the player can select as a reward, uses the item_id. |
| reward_item_quantity | Real     | The quantity of the item to reward.                 |

Adds a reward item to the quest. You can have multiple quest reward items.

### Example:

```
-- Create our quests
QuestCreate("kill_quest")

-- Add reward items for the quest
QuestAddReward("kill_quest","pills_anti_rad",1)
QuestAddReward("kill_quest","medikit_1",1)
```

The above code creates a new quest and adds 2 item rewards to it.