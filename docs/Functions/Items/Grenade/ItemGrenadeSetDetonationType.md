# ItemGrenadeSetDetonationType

### Syntax

`ItemGrenadeSetDetonationType(item_id, type);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description** |
|---|---|---|
| item_id | String | The name of the item to adjust. |
| type | String | One of the values listed below |

Changes how targets are impacted by a grenade.

| Accepted Values: |
|---|
| "GRENADE_detonation_explosion" |
| "GRENADE_detonation_stun" |
| "GRENADE_detonation_flash" |
| "GRENADE_detonation_smoke" |

### Example:

```
ItemGrenadeSetDetonationType("example grenade", "GRENADE_detonation_flash")
```

The above code will change the grenade *"example grenade"* so that when it is used the explosion sprite drawn will be the flash style and rather than doing damage anyone looking at the grenade will have the flash effect applied.