# ItemInjectorCreate

### Syntax

`ItemInjectorCreate(item_id);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| item_id      | String   | The name that can be used to refer to it in the future. |

Create a new medical item that can be affected and referred to by its *<strong>item_id</strong>*. Medical items by default can be used to give the player back HP, remove bleed from the player, cure radiation the player has, restore any max health that has been lost.

### Example:

```
ItemInjectorCreate("Daves Test Injector")
SpriteLoad("Daves Injector Image","test_item.png",1,0,0,0)
ItemSetSpriteInventory("Daves Test Injector","Daves Injector Image")
ItemSetSpriteIngame("Daves Test Injector","Daves Injector Image")
ItemSetName("Daves Test Injector", "Example Medical Item")
ItemInjectorSetDuration("Daves Test Injector",7200)
ItemSetStackLimit("Daves Test Injector",10)
ItemInjectorSetHungerRegen("Daves Test Injector",300)
ItemInjectorSetThirstRegen("Daves Test Injector",300)
```

The above code will create a new injector item that can be spawned in the future and referred to as: "Daves Test Injector". It will have the icon "test_item.png" and over the course of 2 minutes it will slowly recover 30 Hunger and 30 Thirst.

### Default values that can be updated:

| Key:         | Value: |
| :----------- | :----- |
| stack_max    | 3      |
| bleed_immune | false  |
| bleed_rec    | 0      |
| duration     | 14400  |
| hp_regen     | 0      |
| hunger       | -10    |
| hunger_regen | -10    |
| max_hp       | 0      |
| max_weight   | 0      |
| rad_def      | 0      |
| rad_regen    | 0      |
| stamina_max  | 40     |
| stamina_regen| 100    |
| thirst       | -10    |
| thirst_regen | -15    |
| value        | 0      |
| weight       | 0.1    |
| can_be_sold  | true   |