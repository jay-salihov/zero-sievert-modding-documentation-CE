# ItemKeyCreate

### Syntax

`ItemKeyCreate(item_id, single_use);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               | **Default** |
| :----------- | :------- | :-------------------------------------------- | :---------- |
| item_id      | String   | The name that can be used to refer to it in the future. |             |
| single_use   | true/false | Does this item get removed after use.         | true        |

Create a new key item that can be affected and referred to by its *item_id*.

### Example:

```
ItemKeyCreate("Dave Door Key",false)
SpriteLoad("Dave Key","test_item.png",1,0,0,0)
ItemSetSpriteInventory("Dave Door Key","Dave Key")
ItemSetSpriteIngame("Dave Door Key","Dave Key")
ItemSetName("Dave Door Key", "Key for Dave's House")
```

The above code will create a new key item that can be spawned in the future and referred to as: "Dave Door Key". It will have the icon "test_item.png" and can be used many times.