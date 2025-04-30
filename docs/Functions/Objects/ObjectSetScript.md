# ObjectSetScript

### Syntax

`ObjectSetScript(object_id,event_id,event_function);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                                                                             |
| :----------- | :------- | :---------------------------------------------------------------------------------------------------------- |
| object_id    | String   | The ID to use when referring to the object later.                                                           |
| event_id     | String   | The ID for the event that you want to assign a function to. You can find all the available events here: [Player and Object Events](Player and Object Events) |
| event_function | String   | The function to assign to this event.                                                                     |

Assigns a function to an event on an object. This can be used to write custom draw events or step events for example.

### Example:

```
-- Create our new object
ObjectCreate("test_object")

-- Assign a function to the new object
ObjectSetScript("test_object","create_event",func(_inst)
	{
		_inst.sprite_index = SpriteGet("test_sprite")
		_inst.depth = -_inst.y
	})
```

The above code will create a new object and then assign a function to its create event.