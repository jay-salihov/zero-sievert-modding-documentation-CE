# ItemHeadsetCreate

### Syntax

`ItemHeadsetCreate(item_id);`

**Returns** “* **true** *“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                   |
| :----------- | :------- | :------------------------------------------------ |
| item_id      | String   | The name that can be used to refer to it in the future. |

This function creates a new headset item that can be referred to by its * **item_id** *. Headsets can be equipped by the player and then toggled on/off for an on screen effect which normally is used to help see in the dark. By default a headset item will produce a light when turned on (light: *headset_lamp_1*) however this can be changed. For a full list see: [ItemHeadsetSetLightID](ItemHeadsetSetLightID)

The headset can either be used to produce a directional light or it can be used to toggle on a full screen effect which Please note, as well as being able to produce a light it can be used to turn on a screen overlay to give a night vision effect.

If you want the headset to display a light sprite * **ItemHeadsetSetType** * must be set to "torch" and then * **ItemHeadsetSetLightID** * can be used to select the sprite being drawn.

If you want the headset to display an on screen overlay * **ItemHeadsetSetType** * must be set to "night_vision" and then * **ItemHeadsetSetVisionValues** * can be used to adjust the screen values.

##### Torch example:

<span><img/></span>

##### Night Vision example:

<span><img/></span>

### Example:

```
ItemHeadsetCreate("new red head lamp")
ItemHeadsetSetType("new red head lamp","night_vision")
ItemHeadsetSetVisionValues("new red head lamp",1,0,0,0,0,1,0)
```

The above code will create a new headset item that can be spawned in the future and referred to as: "new red head lamp". When equipped and turned on it will give a red overlay on the screen that can be seen in the image above.

### Default values that can be updated:

| Key:         | Value:           | Notes:                                   |
| :----------- | :--------------- | :--------------------------------------- |
| stack_max    | 1                |                                          |
| value        | 6000             |                                          |
| weight       | 0.3              |                                          |
| can_be_sold  | true             |                                          |
| torch_sprite | "headset_lamp_1" | Only used when *type* = "torch"          |
| red          | 1                | Only used when *type* = "night_vision"   |
| blue         | 1                | Only used when *type* = "night_vision"   |
| green        | 1                | Only used when *type* = "night_vision"   |
| brightness   | 0                | Only used when *type* = "night_vision"   |
| contrast     | 0                | Only used when *type* = "night_vision"   |
| gamma        | 1                | Only used when *type* = "night_vision"   |
| grain        | 0                | Only used when *type* = "night_vision"   |