# ScriptExpose

### Syntax

`ScriptExpose(script_name, function);`

**Returns** nothing;

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| `script_name`  | String   | The name of the script to execute.            |
| `function`   | Function | The function to expose.                       |

Exposes a function to other mods. These can be called with [ScriptGet](ScriptGet).

### Example:

```
-- Expose a new script
ScriptExpose("AddTwoValues",func(a,b) {
  return a + b;
});

-- Get and execute our new script
let _addtwovalues = ScriptGet("AddTwoValues")
ShowMessage("Result: " + String(_addtwovalues(5,5)));
```

Creates, exposes, and then executes a script.