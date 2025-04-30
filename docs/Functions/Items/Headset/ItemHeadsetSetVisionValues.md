# ItemHeadsetSetVisionValues

### Syntax

`ItemHeadsetSetVisionValues(item_id, red, green, blue, brightness, contrast, gamma, grain);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description** | Default |
|---|---|---|---|
| item_id | String | The name of the item to update. |  |
| red | Decimal | Amount of red that gets displayed. | 1 |
| green | Decimal | Amount of green that gets displayed. | 1 |
| blue | Decimal | Amount of blue that gets displayed. | 1 |
| brightness | Decimal | Brightness of screen overlay. | 0 |
| contrast | Decimal | Contrast of the screen overlay. | 0 |
| gamma | Decimal | Gamma of the screen overlay. | 1 |
| grain | Decimal | Amount of random noise added to the screen. | 0 |

As long as **ItemHeadsetSetType()** has been set to "night_vision" this can be used to effect how the screen looks.

Please note that while the ranges for these values are generally between 0 and 1 these all accept values outside of those ranges for extreme effects. For example:

### Red:

**Default view:**<br/>
<span><img/></span>

**Red value set to 0:**<br/>
<span><img/></span>

**Red value set to 2:**<br/>
<span><img/></span>

Above shows values of **Red** going from 0 to 2. Using this can either add or remove the red colour from the screen.

### Grain:

Grain 0.1:<br/>
<span><img/></span>

Grain 0.5:<br/>
<span><img/></span>

Grain 1:<br/>
<span><img/></span>

### Brightness:

Brightness -0.5:<br/>
<span><img/></span>

Brightness 0.5:<br/>
<span><img/></span>

### Gamma:

Gamma 0.5:<br/>
<span><img/></span><br/>
Gamma 1.5:<br/>
<span><img/></span>

### Contrast:

Contrast 1:<br/>
<span><img/></span>

Contrast -0.5:<br/>
<span><img/></span>