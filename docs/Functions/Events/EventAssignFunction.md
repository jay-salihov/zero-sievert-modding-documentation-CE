# EventAssignFunction

### Syntax

`EventAssignFunction(event_hook_id,function);`

**Returns** nothing;

| **Argument** | **Type** | **Description**                                         |
| :----------- | :------- | :------------------------------------------------------ |
| event_hook_id | String   | A name to use as a reference to the quest.            |
| function     | Function | An item that the player can select as a reward, uses the item_id. |

Assigns a function a event. This is how you might spawn in an NPC when you enter the bunker or spawn a pet next to the player for example.

### Example:

```
EventAssignFunction("enter_hub",func() { ShowMessage("TEST") }) 
```

The above code assigns a function to the "enter_hub", when you enter the hub a popup message will say "TEST" on the screen.