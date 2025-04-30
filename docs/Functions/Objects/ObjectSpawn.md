# ObjectSpawn

### Syntax

`ObjectSpawn(object_id,x,y);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                   |
| :----------- | :------- | :------------------------------------------------ |
| object_id    | String   | The ID to use when referring to the object later. |
| x            | Real     | The X position of the object.                     |
| y            | Real     | The Y position of the object.                     |

Spawns an object into the world at a position you define.

### Example:

```
-- Create our new object
ObjectCreate("test_object")
-- Spawns an object
ObjectSpawn("test_object",400,400)
```

The above code will create a new object and then spawn it somewhere.