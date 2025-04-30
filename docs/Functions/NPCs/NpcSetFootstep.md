# NpcSetFootstep

### Syntax

`NpcSetFootstep(npc_id,footstep_type);`

**Returns** nothing.

| **Argument**     | **Type** | **Description**                      |
| :--------------- | :------- | :----------------------------------- |
| npc_id         | String   | The NPC ID that should be used.     |
| footstep_type | Real     | The footstep type, a number between 0 and 5. |

Sets the type of footstep sound for this NPC.

| Footstep Value | Description |
| :------------- | :---------- |
| 0              | No sound    |
| 1              | Human       |
| 2              | Wolf        |
| 3              | Boar        |
| 4              | Ghoul       |
| 5              | Big         |

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Set the type of footsteps this NPC uses to use the boar sounds
NpcSetFootstep("test_npc",3)
```

The above code will create a NPC and then set its footstep sounds.