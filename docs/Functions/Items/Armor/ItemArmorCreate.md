# ItemArmorCreate

### Syntax

`ItemArmorCreate(item_id);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| item_id      | String   | The name that can be used to refer to it in the future. |

Create a new armor that can be affected and referred to by its *<strong>item_id</strong>*. Armor can be equipped by the player to change the amount of damage and radiation they take.

### Example:

```
ItemArmorCreate("Daves Test Armor")
SpriteLoad("example sprite icon","test-sprite-icon.png",1,0,0,0)
SpriteLoad("example sprite world","test-sprite-world.png",1,0,0,0)

ItemSetSpriteInventory("Daves Test Armor","example sprite icon")
ItemArmorSetSpriteDead("Daves Test Armor","example sprite world")
ItemArmorSetSpriteIdle("Daves Test Armor","example sprite world")
ItemArmorSetSpriteRun("Daves Test Armor","example sprite world")

ItemArmorSetAnomaly("Daves Test Armor",10)
ItemArmorSetClass("Daves Test Armor",3)
ItemArmorSetFragility("Daves Test Armor",26)
ItemArmorSetPierce("Daves Test Armor",0.28)
ItemArmorSetRadiation("Daves Test Armor",15)
```

The above code will create a new armour item that can be spawned in the future and referred to as: "Daves Test Armor". It will have the inventory icon "test-sprite-icon.png" and when the player has it equipped it will draw "test-sprite-world.png". It can be equipped in the armor slot.

### Default values that can be updated:

| Key:        | Value:                  |
| :---------- | :---------------------- |
| anomaly     | 0                       |
| class       | 1                       |
| fragility   | 2                       |
| pierce      | 0.1                     |
| rediation   | 0                       |
| value       | 7000                    |
| weight      | 2                       |
| max_stack   | 1                       |
| can_be_sold | true                    |
| sprite_dead | "s_bandit_novice_dead"  |
| sprite_idle | "s_bandit_novice_idle"  |
| sprite_run  | "s_bandit_novice_run"   |