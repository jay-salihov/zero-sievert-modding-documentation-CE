# WeaponModScopeConfigure

### Syntax

```
WeaponModScopeConfigure(item_id, scope_is_optic=false, glance_mouse_distance_multiplier=1.15, _scope_extend_view_multiplier=1.25, _scope_effective_range_multiplier=1.25);
```

**Returns** undefined.

| **Argument**                      | **Type** | **Description**                                                                  |
| --------------------------------- | -------- | -------------------------------------------------------------------------------- |
| item_id                           | String   | A name to use as a reference to the item.                                       |
| scope_is_optic                    | Boolean  | Whether or not the view will scope in using a sprite. Generally this means the screen is black besides the area around the cursor. |
| glance_mouse_distance_multiplier  | Real     | Affects the distance crosshair-target within a perfect shot is possible.        |
| scope_extend_view_multiplier      | Real     | Affects the range that the view can be extended while zoomed in.                |
| scope_effective_range_multiplier  | Real     | Affects the effective range of the weapon while zoomed in.                       |

You can use this function to modify the various values that a weapon scope utilizes.

### Example:

```
-- Now create a weapon mod, scope
WeaponModCreate("mod_test_scope", "scope", 0, 0, 0, 0, 0, false, ["test_weapon"])
-- Now configure the scope
WeaponModScopeConfigure("mod_test_scope",false,1.25,1.25,1.25)
```

The above code creates a new weapon mod that is a scope, and then configures the values for that weapon mod.