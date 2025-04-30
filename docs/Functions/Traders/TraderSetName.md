# TraderSetName

### Syntax

`TraderSetName(trader_id="Default", name);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                        |
| :----------- | :------- | :------------------------------------- |
| trader_id    | String   | The ID of trader to modify.            |
| name         | Real     | The name shown for the trader. |

Modifies the name shown for the trader.

### Example:

```
-- Create our new trader
TraderCreate("test_trader")

-- Set the name shown for the trader
TraderSetName("test_trader","A Legit Trader Guy")
```

The above code will create a new trader and then set the name that is shown to "A Legit Trader Guy".