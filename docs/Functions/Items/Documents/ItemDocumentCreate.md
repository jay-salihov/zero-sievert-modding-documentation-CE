# ItemDocumentCreate

### Syntax

`ItemDocumentCreate(item_id, single_use);`

**Returns** “*true*“, if successful, otherwise it will crash.

**IMPORTANT: This function has been deprecated.**

| **Argument** | **Type** | **Description**                                        | **Default** |
| :----------- | :------- | :----------------------------------------------------- | :---------- |
| item_id      | String   | The name that can be used to refer to it in the future. |             |
| reputation   | Real     | Amount of reputation gained.                           | 1           |

Create a new document item that can be affected and referred to by its *item_id*.

### Example:

```
ItemDocumentCreate("Blue Document",3)
SpriteLoad("Sprite Blue Document","test_item.png",1,0,0,0)
ItemSetSpriteInventory("Blue Document,"Sprite Blue Document")
ItemSetSpriteIngame("Blue Document","Sprite Blue Document")
ItemSetName("Blue Document", "Big Blue Document")
```

The above code will create a new key item that can be spawned in the future and referred to as: "Blue Document". It will have the icon "test_item.png" and gives 3 reputation.