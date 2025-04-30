# ItemMedicalCreate

### Syntax

`ItemMedicalCreate(item_id, hp_healed, radiation_healed, sound_name);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument**    | **Type** | **Description**                                  | **Default**     |
| :-------------- | :------- | :----------------------------------------------- | :-------------- |
| item_id         | String   | The name that can be used to refer to it in the future. |                 |
| hp_healed       | Real     | The amount of HP the player will recover over the duration of the item. | 0               |
| sound_name      | String   | The sound that gets played when this is consumed. | "snd_medikit_1" |

Create a new medical item that can be affected and referred to by its *<strong>item_id</strong>*. Medical items by default can be used to give the player back HP, remove bleed from the player, cure radiation the player has, restore any max health that has been lost.

### Example:

```
ItemMedicalCreate("Example Medical Item",50)
SpriteLoad("Example medical icon","test_item.png",1,0,0,0)
ItemSetSpriteInventory("Example Medical Item","Example medical icon")
ItemSetSpriteIngame("Example Medical Item","Example medical icon")
ItemSetName("Example Medical Item", "Example Medical Item")
ItemMedicalSetDuration("Example Medical Item",120)
ItemSetStackLimit("Example Medical Item",10)
ItemMedicalSetBleed("Example Medical Item",5)
```

The above code will create a new medical item that can be spawned in the future and referred to as: "Example medical icon". It will have the icon "test_item.png" and over the course of 2 seconds will recover 50 HP and cure 5 stacks of bleed.

### Default values that can be updated:

The default animation that will be played while the player is consuming this item will be "s_arms_med1" however this can be changed with `ItemMedicalSetAnimation()`

| Key:             | Value: | Description:                                                                                                |
| :--------------- | :----- | :---------------------------------------------------------------------------------------------------------- |
| radiation        | 0      | How many stacks of radiation does this remove.                                                              |
| bleed            | 0      | How many stacks of bleed does this remove.                                                                  |
| wound            | 0      | If the player has lost max HP how much of it is recovered.                                                  |
| duration         | 30     | How long it takes to fully consume this item in frames. <br/>Note: *The game runs at 60 fps so 30 would be half a second.* |
| can_move         | true   | While this item is being consumed can the player move. (true/false)                                         |
| speed_multiplier | 0.5    | While the item is being consumed what speed the player can move at.                                         |
| stack_max        | 10     | Maximum quantity of this item that can be in one slot in the inventory.                                      |
| value            | 0      | How much this item sells for at traders.                                                                    |
| weight           | 0.05   | The weight of this item when carried by the player.                                                         |
| can_be_sold      | true   | Can the player sell this item to traders (true/false)                                                        |

### Helpful functions:

[ItemMedicalSetAnimation]()<br/>
[ItemMedicalSetBleed]()<br/>
[ItemMedicalSetWound]()<br/>
[ItemMedicalSetRadiation]()<br/>
[ItemMedicalSetMoveSpeedMultiplier]()<br/>
[ItemMedicalSetDuration]()<br/>
[ItemMedicalSetCanMove]()