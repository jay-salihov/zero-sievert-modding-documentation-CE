# NpcSetWeapon

### Syntax

`NpcSetWeapon(npc_id,weapon);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                  |
| :----------- | :------- | :----------------------------------------------- |
| npc_id       | String   | The NPC ID that should be used.                 |
| weapon       | String   | The item ID of the weapon this NPC should use. |

Assigns a specific weapon/item to an NPC to be used as a waepon.

There are two additional values that are accepted instead of a weapon/item ID.
`no_weapon` for humans and `no_item` for non-humans.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Assign our NPC a weapon
NpcSetWeapon("test_npc","akm")
```

The above code will create a NPC and then assign it the item "akm" to use as a weapon.