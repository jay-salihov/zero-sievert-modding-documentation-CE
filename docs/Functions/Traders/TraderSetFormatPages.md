# TraderSetFormatPages

### Syntax

`TraderSetFormatPages(trader_id="Default", format_pages);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| trader_id    | String   | The ID of trader to modify.                   |
| format_pages | Boolean  | The name of the faction this trader belongs to. |

Modifies whether or not the trading page is formatted.

### Example:

```
-- Create our new trader
TraderCreate("test_trader")
-- Set the faction for the trader
TraderSetFormatPages("test_trader",true)
```

The above code will create a new trader and set it to format its pages.