# WeaponModLaserConfigure

### Syntax

`WeaponModLaserConfigure(item_id, laser_color_rgb=[255,255,255]);`

**Returns** undefined.

| **Argument** | **Type** | **Description**                                    |
|--------------|----------|----------------------------------------------------|
| item_id      | String   | A name to use as a reference to the item.        |
| laser_color_rgb| Array    | This is an array of 3 color values. Red, green, and blue. |

You can use this function to modify the color of the laser.

### Example:

```
-- Now create a weapon mod, laser
WeaponModCreate("mod_test_laser", "laser", 0, 0, 0, 0, 0, false, ["test_weapon"])
-- Now configure the laser
WeaponModLaserConfigure("mod_test_laser",[255,255,255])
```

The above code creates a new weapon mod that is a laser, and then configures the color of that laser. In this case the color is pure white.