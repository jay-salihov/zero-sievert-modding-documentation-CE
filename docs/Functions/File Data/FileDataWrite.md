# FileDataWrite

### Syntax

`FileDataWrite(key,value);`

**Returns** undefined.

| **Argument** | **Type**        | **Description**                         |
| :----------- | :-------------- | :-------------------------------------- |
| key          | String          | The key for referencing the data later. |
| value        | Real/String/Array/Struct | The value to be saved.                  |

Writes a value to the save data which will be saved to the game save file and can be read at any time with [FileDataRead](FileDataRead).

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