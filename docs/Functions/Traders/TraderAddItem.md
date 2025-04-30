# TraderAddItem

### Syntax

```
TraderAddItem(trader_id="Default", item_id, quantity=1, faction_level=undefined, quest_requirement=undefined);
```

**Returns** nothing.

| **Argument**       | **Type** | **Description**                                                                                                |
| ------------------ | -------- | -------------------------------------------------------------------------------------------------------------- |
| trader_id          | String   | The ID of trader to modify.                                                                                    |
| item_id            | String   | The ID of the item to add.                                                                                     |
| quantity           | Real     | The amount of the item that should be kept in stock.                                                            |
| faction_level      | Real     | The relationship value required to be had with this traders faction. If *undefined*, there will be no quest requirement. |
| quest_requirement | String   | The ID of the quest to use as a requirement. If *undefined*, there will be no quest requirement.                |

Adds an item to a traders inventory.

### Example:

```
-- Create our new trader
TraderCreate("test_trader")

-- Adds items to the trader
TraderAddItem("test_trader","aa12",1,undefined,undefined)
TraderAddItem("test_trader","anti_bleed_gel",1,150,undefined)
```

The above code will create a new trader and then adds 2 items to their inventory.