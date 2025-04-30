# NpcObjectDestroy

### Syntax

`NpcObjectDestroy(instance_id);`

**Returns** nothing.

| **Argument** | **Type**      | **Description**                                                                  |
| :----------- | :------------ | :------------------------------------------------------------------------------- |
| instance_id  | Instance ID | The instance to destroy (should be an instance of a NPC object). |

Deletes an instance of a NPC object without triggering all of the effects of killing that NPC. For example, won't reward the player with XP. This can be helpful for clearing enemies off of the map.

### Example:

```
ObjectSetScript("obj_player","step_normal_event",func(_inst) {
  if ( RoomGetCurrent() != "r_hub" ) {
    let _array = ObjectGetAllInstances(obj_npc_parent)
    let _index = 0
    while ( _index < ArrayLength(_array) ) {
      NpcObjectDestroy(_array[_index])
      _index += 1
    }
  }
});
```

The above code will remove all NPCs from the map every frame if the player is in a non-hub level.