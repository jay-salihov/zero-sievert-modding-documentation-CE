# Object Events

When creating objects you are given the option of assigned functions to various events that are performed by the object. Below is a list of all the available events and when/how they are called.

| **Event ID**        | **Description**                                                                |
| :------------------ | :----------------------------------------------------------------------------- |
| "create_event"      | Called once when the object is spawned.                                       |
| "step_begin_event"  | Called every step (frame) of the game, before the "step_normal_event".        |
| "step_normal_event" | Called every step (frame) of the game, before the "step_end_event".          |
| "step_end_event"    | Called every step (frame) of the game, after the "step_normal_event".         |
| "draw_normal_event" | Called every step (frame) of the game, after the "step_end_event".          |
| "draw_end_event"    | Called every step (frame) of the game, after the "draw_end_event".           |
| "destroy_event"     | Called when the instance is destroyed.                                       |
| "cleanup_event"     | Called when the instance is destroyed and is used to cleanup code even when it's destroyed by methods that aren't InstanceDestroy(). |