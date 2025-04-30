# NpcSetPreset

### Syntax

`NpcSetPreset(npc_id,preset);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                                                                                                                                                                                                                                                                                                                                   |
| :----------- | :------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| npc_id       | String   | The NPC ID that should be used.                                                                                                                                                                                                                                                                                                                                |
| preset       | String   | The preset to use for this NPC. You can find a list of available presets here [NPC Presets](NPC Presets).                                                                                                                                                                                                                                                          |

Assigns a preset to be used by the NPC. There are a lot of attributes that NPCs use and in place of those values you can use, `{use_preset}`.

### Example:

```
-- Create our NPC
NpcCreate("test_npc")

-- Assign our NPC a preset to use
NpcSetPreset("test_npc","crimson_master")
```

The above code will create a NPC and then assigns it a preset to use.