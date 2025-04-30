# Real

### Syntax

`Real(value);`

**Returns** the value as a real.

| **Argument** | **Type**     | **Description**                                  |
| :----------- | :----------- | :----------------------------------------------- |
| value        | String/Real | The value you would like to return as a real. |

Returns the value provided as a real. For example, passing in a value like "abc123", it would return it as "123".

### Example:

```
ShowMessage("The number is " + String(Real("blah blah 10")));
```

The above code will popup a message that says "The number is 10".