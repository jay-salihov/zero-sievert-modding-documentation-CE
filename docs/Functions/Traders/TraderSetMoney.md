# TraderSetMoney

### Syntax

`TraderSetMoney(trader_id="Default", money);`

**Returns** nothing.

| **Argument** | **Type** | **Description** |
|---|---|---|
| trader_id | String | The ID of trader to modify. |
| money | Real | The amount of money the trader has. |

Modifies the amount of money that the trader has.

### Example:

```
-- Create our new trader
TraderCreate("test_trader")
-- Set the amount money that the trader as
TraderSetMoney("test_trader",true)
```

The above code will create a new trader and then set the amount of money that it has.