# ItemSetPriceValue

### Syntax

`ItemSetPriceValue(item_id, price_value);`

**Returns** “*true*“, if successful, otherwise it will crash.

| Argument    | Type   | Description                    |
| ----------- | ------ | ------------------------------ |
| item_id     | String | The name of the item to adjust. |
| price_value | Real   | The price value of the item.   |

Changes the price value of the item.

### Example:

```
-- Modify the price of the bandage item
ItemSetPriceValue("bandage", 100)
```

The above code will change the price of the item to 100 roubles.