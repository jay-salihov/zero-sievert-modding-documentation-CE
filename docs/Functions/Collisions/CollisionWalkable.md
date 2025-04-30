# CollisionWalkable

### Syntax

`CollisionWalkable(x,y);`

**Returns** true or false.

| **Argument** | **Type** | **Description**           |
| :----------- | :------- | :----------------------    |
| x            | Real     | The x position to check.  |
| y            | Real     | The y position to check.  |

Checks if a position is walkable for an NPC.

### Example:

```
if ( CollisionWalkable(30,30) ) { ShowMessage("Walkable!") }
```

The above code check if a position is walkable.