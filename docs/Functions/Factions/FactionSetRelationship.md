# FactionSetRelationship

### Syntax

`FactionSetRelationship(faction_a,faction_b,relationship_value);`

**Returns** undefined.

| **Argument**       | **Type** | **Description**                                                                                                    |
| ------------------ | -------- | ------------------------------------------------------------------------------------------------------------------ |
| faction_a          | String   | The id of the first faction that we are affecting.                                                                 |
| faction_b          | String   | The id of the second faction that we are affecting.                                                                |
| relationship_value | Real     | This value determines how faction relations. See [Faction Reputation](Faction Reputation) for a list of macros and expected behaviors. |

Changes the relationship value between two factions. This can make them neutral, allies, or enemies. You can also find a list of all of the integrated factions that are included in the base game on this page: [Faction Names](Faction Names)

### Example:

```
-- Create a faction
FactionCreate("new_faction")
-- Set the new factions relationship status with the player
FactionSetRelationship("new_faction","Player",FACTION_REP_ENEMY)
```

The above code creates a new faction and sets the factions relationship status with the player to be enemies (250).