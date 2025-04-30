# ChestSetItemDropChance

### Syntax

`ChestSetItemDropChance(chest_id,chance_uncommon,chance_rare,chance_legendary,chance_epic);`

**Returns** undefined.

| **Argument**     | **Type** | **Description**                                           |
| :--------------- | :------- | :-------------------------------------------------------- |
| chest_id         | String   | The chest ID to modify.                                   |
| chance_uncommon  | Real     | The chance of getting a drop of this rarity. (0 - 100)    |
| chance_rare      | Real     | The chance of getting a drop of this rarity. (0 - 100)    |
| chance_legendary | Real     | The chance of getting a drop of this rarity. (0 - 100)    |
| chance_epic      | Real     | The chance of getting a drop of this rarity. (0 - 100)    |

Sets the drop chance for each rarity. Each item that is added can have a rarity set specifically for this chest. See [ChestAddItem](/Functions/Chests/ChestAddItem.md) for more information.

### Example:

```
-- Create a chest
ChestCreate("new_chest")
-- Set the drop rates for items
ChestSetItemDropChance("new_chest",40,30,20,10)
```

The above code creates a new chest and then sets the drop rates of items.