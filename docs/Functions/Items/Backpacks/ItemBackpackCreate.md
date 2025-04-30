# ItemBackpackCreate

### Syntax

`ItemBackpackCreate(item_id);`

**Returns** “* **true** *“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                 |
| :----------- | :------- | :---------------------------------------------- |
| item_id      | String   | The name that can be used to refer to it in the future. |

Create a new backpack that can be affected and referred to by its * **item_id** *. Backpacks can be equipped by the player to change the amount of weight they can carry.

### Example:

```
ItemBackpackCreate("Daves Test Backpack")
SpriteLoad("Daves Test Image icon","test-icon.png",1,0,0,0)
SpriteLoad("Daves Test Image world","test-world.png",1,0,0,0)
ItemSetSpriteInventory("Daves Test Backpack","Daves Test Image")
ItemBackpackSetSpriteGame("Daves Test Backpack","Daves Test Image")
ItemBackpackSetWeight("Daves Test Backpack","100")
```

The above code will create a new backpack item that can be spawned in the future and referred to as: "Daves Test Backpack". It will have the inventory icon "test-icon.png" and when the player has it equipped it will draw "test-world.png". It can be equipped in the backpack slot and when it is it will increase the weight of items that can be carried by 100.

### Default values that can be updated:

| Key:            | Value:                  |
| :-------------- | :---------------------- |
| ergonomic       | 0                       |
| movement_speed  | 0                       |
| sprite_game     | s_item_backpack_un_game |
| weight          | 0                       |
| carry weight    | 20                      |
| value           | 25000                   |