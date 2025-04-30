# LanguageCreate

### Syntax

`LanguageCreate(language_id,language_display_name,csv_file,font_file)`

**Returns** nothing.

| **Argument**           | **Type** | **Description**                                                                                                                                                                                             |
| ---------------------- | -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| langauge_id            | String   | The ID to use when referring to the language later.                                                                                                                                                         |
| language_display_name  | String   | The name displayed for the language in the language settings menu.                                                                                                                                          |
| csv_file               | String   | The name (a string file path) of the file to add. The CSV file should resemble the same format as the other CSV language which can be found in the game files.                                             |
| font_file              | String   | The name (a string file path) of the file to add.                                                                                                                                                           |

Creates a new language that can be selected from the language settings menu.

### Example:

```
LanguageCreate("russian","Русский (Russian)","russian.csv","silver.ttf")
LanguageSetFontSizes("russian",[13,15,18,27,36,68])
LanguageSetFontOffsets("russian",[
    {x : 0, y : 2, linebreak_height : 18},
    {x : 0, y : 2, linebreak_height : 20},
    {x : 0, y : 3, linebreak_height : 23},
    {x : 0, y : 5, linebreak_height : 32},
    {x : 0, y : 6, linebreak_height : 41},
    {x : 0, y : 10, linebreak_height : 73}
])
```

The above code will create a new language and configure the font.