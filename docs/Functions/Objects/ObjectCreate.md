# ObjectCreate

### Syntax

`ObjectCreate(object_id);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                    |
| :----------- | :------- | :------------------------------------------------- |
| object_id    | String   | The ID to use when referring to the object later. |

Creates a new object that you can place into the world. This object can have events and behave like any other object in the world.

### Example:

```
-- Create our new object
ObjectCreate("test_object")
```

The above code will create a new object.