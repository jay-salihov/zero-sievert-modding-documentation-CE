# RoomGetCurrent

### Syntax

`RoomGetCurrent();`

**Returns** the name of the current room.

| **Argument** | **Type** | **Description** |
| ----------- | ----------- | ----------- |
| N/A | N/A | N/A |

Returns the name of the room you are currently in.

### Example:

```
if ( RoomGetCurrent() == "r_hub" ) { ShowMessage("Hello!"); }
```

The above code will popup a message that says "Hello!" when we the room is currently "r_hub".