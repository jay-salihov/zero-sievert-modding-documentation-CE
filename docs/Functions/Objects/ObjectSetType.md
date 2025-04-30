# ObjectSetType

### Syntax

`ObjectSetType(object_id,object_type);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                             |
| :----------- | :------- | :---------------------------------------------------------- |
| object_id    | String   | The ID to use when referring to the object later.           |
| object_type  | String   | The type of object that this custom object should use.      |

Allows you to change the type of object that this custom object uses. For example, you can have a non-collision object with "obj_mod_generic" or one that can be collided with "obj_mod_generic_solid". Here you can find all of the [Object Types](Object Types) available.

### Example:

```
-- Create our new object
ObjectCreate("test_object")
-- Assign an object a specific type to use as a template
ObjectSetType("test_object","obj_mod_generic_solid")
```

The above code will create a new object and then give it a different object type to use.