# Player and Object Events

When creating objects you are given the option of assigned functions to various events that are performed by the object. Below is a list of all the available events and when/how they are called.

| **Event ID**        | **Description**                                                              |
| :------------------ | :--------------------------------------------------------------------------- |
| "create_event"      | Called once when the object is spawned.                                     |
| "step_begin_event"  | Called every step (frame) of the game, before the "step_normal_event".      |
| "step_normal_event" | Called every step (frame) of the game, before the "step_end_event".        |
| "step_end_event"    | Called every step (frame) of the game, after the "step_normal_event".       |
| "draw_normal_event" | Called every step (frame) of the game, after the "step_end_event".         |
| "draw_end_event"    | Called every step (frame) of the game, after the "draw_end_event".         |
| "destroy_event"     | Called when the instance is destroyed.                                      |
| "cleanup_event"     | Called when the instance is destroyed and is used to cleanup code even when it's destroyed by methods that aren't InstanceDestroy().                                     |

All of these events will pass along the instance id of the instance that is calling them. See the example below and how the `_inst` argument is used. In the example below, the `_inst` argument is the `obj_player`'s instance id.

```lua
-- Bind a function to our create event
ObjectSetScript("obj_player","create_event",func(_inst)
{
    _inst.radius = 192
    _inst.spawn_rate = 60 * 1
    _inst.spawn_timer = 0
});

-- During our step event, spawn boars
ObjectSetScript("obj_player","step_normal_event",func(_inst)
{
    if ( RoomGetCurrent() != "r_hub" )
    {
        _inst.spawn_timer += 1
        if ( _inst.spawn_timer >= _inst.spawn_rate )
        {
            let _dir = Irandom(360);
            let _dist = 240;

            -- Spawn a boar
            if ( CollisionWalkable(_inst.x + LengthDirX(_dist,_dir),_inst.y + LengthDirY(_dist,_dir)) )
            {
                InstanceCreate(_inst.x + LengthDirX(_dist,_dir),_inst.y + LengthDirY(_dist,_dir),obj_enemy_boar)
                _inst.spawn_timer = 0
            }
        }
    }
});
```