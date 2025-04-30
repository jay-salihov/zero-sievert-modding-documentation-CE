# ChestAddItem

### Syntax

`ChestAddItem(chest_id,item,rarity);`

**Returns** undefined.

| **Argument** | **Type** | **Description** |
|---|---|---|
| chest_id | String | The chest ID to modify. |
| item | String | The item ID to add. |
| rarity | String | The rarity of the item. You can leave this argument blank to bypass the rarity system for this item. See the rarities listed below. |

Adds a new item to the chest.

| Rarities |
|---|
| "uncommon" |
| "rare" |
| "epic" |
| "legendary" |

### Example:

```
-- Create a chest
ChestCreate("new_chest")

-- Adds an item to the chest
ChestAddItem("new_chest","whisky","uncommon")
```

The above code creates a new chest and then adds an item to it.