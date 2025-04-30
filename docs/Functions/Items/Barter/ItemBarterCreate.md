# ItemBarterCreate

### Syntax

`ItemBarterCreate(item_id, single_use);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                   | **Default** |
| :----------- | :------- | :------------------------------------------------ | :---------- |
| item_id      | String   | The name that can be used to refer to it in the future. |             |

Create a new bartering item that can be affected and referred to by its *item_id*.

### Example:

```
ItemBarterCreate("Daves Junk Item")
SpriteLoad("example sprite","test_item.png",1,0,0,0)
ItemSetSpriteInventory("Daves Junk Item","example sprite")
ItemSetSpriteIngame("Daves Junk Item","example sprite")
ItemSetName("Daves Junk Item", "Big Junk Item")
```

The above code will create a new barter item that can be spawned in the future and referred to as: "Daves Junk Item". It will have the icon "test_item.png" and have the name "Big Junk Item".