# LanguageSetFontOffsets

### Syntax

`LanguageSetFontOffsets(language_id,offset_data)`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                                                                                                               |
| :----------- | :------- | :------------------------------------------------------------------------------------------------------------------------------------------ |
| langauge_id  | String   | The ID of the language you want to modify.                                                                                                  |
| offset_data  | Array    | An array containing 6 struct entries, each containing the x and y offsets of the font at that size, and the vertical space between line breaks. |

Modifies the font offsets for each step up in size. Zero Sievert has 6 font sizes it uses in various places. This allows you to configure the offset and line break height of this font in each of those use cases, from smallest to largest.

### Example:

```
LanguageCreate("russian","Русский (Russian)","russian.csv","silver.ttf")
LanguageSetFontOffsets("russian",[
  {x : 0, y : 2, linebreak_height : 18},
  {x : 0, y : 2, linebreak_height : 20},
  {x : 0, y : 3, linebreak_height : 23},
  {x : 0, y : 5, linebreak_height : 32},
  {x : 0, y : 6, linebreak_height : 41},
  {x : 0, y : 10, linebreak_height : 73}
])
```

The above code will create a new language and configure the font offsets for each font size step.