# TraderCreate

### Syntax

```
TraderCreate(trader_id="Default", faction="All Friend", format_pages=false, money=100000);
```

**Returns** nothing.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| trader_id    | String   | The ID to use when referring to the trader later. |

Creates a new trader that can be assigned to an NPC. You can *not* have duplicate trader IDs.

### Example:

```
-- Create our new trader
TraderCreate("test_trader")
```

The above code will create a new trader.