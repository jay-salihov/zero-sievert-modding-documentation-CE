# TraderSetFaction

### Syntax

`TraderSetFaction(trader_id="Default", faction);`

**Returns** nothing.

| **Argument** | **Type** | **Description** |
|---|---|---|
| trader_id | String | The ID of trader to modify. |
| faction | String | The name of the faction this trader belongs to. |

Modifies the faction assigned to a trader.

### Example:

```
-- Create our new trader
TraderCreate("test_trader")

-- Set the faction for the trader
TraderSetFaction("test_trader","All Friends")
```

The above code will create a new trader and set it's faction to "All Friends".