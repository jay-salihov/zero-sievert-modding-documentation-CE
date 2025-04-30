# ChestSetFromEnemy

### Syntax

```
ChestSetFromEnemy(chest_id,from_enemy);
```

**Returns** undefined.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| chest_id     | String   | The chest ID to modify.                          |
| from_enemy   | Boolean  | Whether or not the chest is dropped by an enemy. |

Used to determine if a chest is dropped by an enemy for game logic.

### Example:

```
-- Create a chest
ChestCreate("new_chest")

-- Set whether or not the chest is dropped by an enemy
ChestSetFromEnemy("new_chest",true)
```

The above code creates a new chest and then sets a flag that says it's dropped by an enemy.