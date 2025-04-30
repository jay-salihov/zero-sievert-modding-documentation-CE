# ItemHeadsetSetType

### Syntax

`ItemHeadsetSetType(item_id, type);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                 |
| :----------- | :------- | :---------------------------------------------- |
| item_id      | String   | The name of the item to update.                 |
| type         | String   | Either "torch" or "night_vision"                |

Headsets can only be either a **"torch"** which draws a sprite in the direction the player is facing, or **"night_vision"** which displays an overlay on the screen.

When in torch mode [ItemHeadsetSetLightID](ItemHeadsetSetLightID) can be used to change the image being displayed.

When in night vision mode [ItemHeadsetSetVisionValues](ItemHeadsetSetVisionValues) can be used to change the values of the screen overlay.

##### Torch example:

<span></span>

##### Night Vision example:

<span></span>