# ScriptGet

### Syntax

`ScriptExpose(script_name, function);`

**Returns** the function of referred to by the `script_name` or throws an error.

| **Argument** | **Type** | **Description** |
|---|---|---|
| `script_name` | String | The name of the script to execute. |
| `function` | Function | The function to expose. |

Returns a script that was previously exposed with [ScriptExpose](ScriptExpose).

### Example:

```
-- Expose a new script
ScriptExpose("AddTwoValues",fun(a,b) { return a + b; });

-- Get and execute our new script
let _addtwovalues = ScriptGet("AddTwoValues")
ShowMessage("Result: " + String(_addtwovalues(5,5)));
```

Creates, exposes, and then executes a script.