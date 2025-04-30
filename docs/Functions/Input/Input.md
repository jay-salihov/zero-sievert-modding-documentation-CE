# Input

The engine that Zero Sievert is built on has some basic input features that can be accessed through the functions listed below. You'll have to follow their documentation. Besides the function names being different, their behaviors work identically.

##### Keyboard Checks

| Functions           | Documentation         |
| ------------------- | --------------------- |
| KeyboardCheck       | <a>keyboard_check</a>   |
| KeyboardCheckPressed  | <a>keyboard_check_presed</a> |
| KeyboardCheckReleased | <a>keyboard_check_released</a> |

##### Mouse Checks

| Functions             | Documentation           |
| --------------------- | ----------------------- |
| MouseCheckButton      | <a>mouse_check_button</a>    |
| MouseCheckButtonPressed | <a>mouse_check_button_pressed</a> |
| MouseCheckButtonReleased| <a>mouse_check_button_released</a>|

##### Keycodes

| Functions | Documentation |
| --------- | ------------- |
| Ord       | <a>ord</a>       |

##### Game Maker Mouse/Keyboard Constants

| Mouse/Keyboard Constants |
| ------------------------ |
| "vk_nokey"               |
| "vk_anykey"              |
| "vk_enter"               |
| "vk_return"              |
| "vk_shift"               |
| "vk_control"             |
| "vk_alt"                 |
| "vk_escape"              |
| "vk_space"               |
| "vk_backspace"           |
| "vk_tab"                 |
| "vk_pause"               |
| "vk_printscreen"         |
| "vk_left"                |
| "vk_right"               |
| "vk_up"                  |
| "vk_down"                |
| "vk_home"                |
| "vk_end"                 |
| "vk_delete"              |
| "vk_insert"              |
| "vk_pageup"              |
| "vk_pagedown"            |
| "vk_f1"                  |
| "vk_f2"                  |
| "vk_f3"                  |
| "vk_f4"                  |
| "vk_f5"                  |
| "vk_f6"                  |
| "vk_f7"                  |
| "vk_f8"                  |
| "vk_f9"                  |
| "vk_f10"                 |
| "vk_f11"                 |
| "vk_f12"                 |
| "vk_numpad0"             |
| "vk_numpad1"             |
| "vk_numpad2"             |
| "vk_numpad3"             |
| "vk_numpad4"             |
| "vk_numpad5"             |
| "vk_numpad6"             |
| "vk_numpad7"             |
| "vk_numpad8"             |
| "vk_numpad9"             |
| "vk_divide"              |
| "vk_multiply"            |
| "vk_subtract"            |
| "vk_add"                 |
| "vk_decimal"             |
| "vk_lshift"              |
| "vk_lcontrol"            |
| "vk_lalt"                |
| "vk_rshift"              |
| "vk_rcontrol"            |
| "vk_ralt"                |
| "mb_any"                 |
| "mb_none"                |
| "mb_left"                |
| "mb_right"               |
| "mb_middle"              |
| "mb_side1"               |
| "mb_side2"               |

### Example:

```
-- Check for keyboard input
if ( KeyboardCheckPressed(Ord("P")) )
{
    ShowMessage("Keyboard")
}

-- Check for mouse input
if ( MouseCheckButtonPressed(mb_left) )
{
    ShowMessage("Test")
}
```