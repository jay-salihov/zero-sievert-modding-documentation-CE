# Items

##### Creating Items

You can quickly create or add new items with [ItemCreate](ItemCreate), however there are also tons of shortcuts for various item types such as [ItemBackpackCreate](ItemBackpackCreate).

##### Item Sprites

Generally the sprites used for items are some multiple of 16x16. This is because the inventory uses a grid system where each cell is 16x16 pixels. Therefor an item that is 32x16 will take up 2x1 cells in the inventory. Be sure to include any necessary empty space around the sprite to keep the total size at some multiple of 16x16.

To assign your own sprites to items, see the example below:

```
-- Load our item sprite
SpriteLoad("test_item","test_item.png",1,0,0,0);

-- Now assign it to our "bandage" item asset
ItemSpriteSetInventory("bandage",SpriteGet("test_item"))
```