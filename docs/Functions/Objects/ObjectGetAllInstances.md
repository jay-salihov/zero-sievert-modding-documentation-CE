# ObjectGetAllInstances

### Syntax

`ObjectGetAllInstances(object);`

**Returns** an array.

| **Argument** | **Type** | **Description**                       |
| :----------- | :------- | :------------------------------------ |
| object       | String   | The object to get all instances of. |

Returns a list of all instances of the defined `object`. Use one of the entries from the [Pre-Existing Objects](Pre-Existing Objects) page for the `object`.

### Example:

```
let _array = ObjectGetAllInstances(obj_enemy_boar)
```

The above code will get an array of all instances of the `obj_enemy_boar` object.