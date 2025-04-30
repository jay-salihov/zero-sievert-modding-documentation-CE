# FileDataRead

### Syntax

`FileDataRead(key);`

**Returns** the value attached to the key or an empty struct.

| **Argument** | **Type** | **Description**                       |
| :----------- | :------- | :------------------------------------ |
| key          | String   | The key for referencing the data later. |

Read a value previously stored in memory.

### Example:

```
ObjectSetScript("obj_player","step_normal_event",func(_inst) {
	let _time = FileDataRead("time")
	if ( _time == undefined ) {
		_time = 0
	}
	FileDataWrite("time",_time + 1)
});
```

Writes a value called "time" to save data and increments it by 1 each frame.