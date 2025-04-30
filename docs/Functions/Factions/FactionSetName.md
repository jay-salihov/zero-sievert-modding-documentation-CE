# FactionSetName

### Syntax

`FactionSetName(faction_id,name);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                               |
| :----------- | :------- | :-------------------------------------------- |
| faction_id   | String   | The id of the faction that we are affecting.  |
| name         | String   | This is the name which may be displayed in the game. |

Changes the name that is displayed in the game for the faction.

### Example:

```
-- Create a faction
FactionCreate("new_faction")
-- Set the faction name
FactionSetName("new_faction","New Faction")
```

The above code creates a new faction and sets the factions in game name to "New Faction".