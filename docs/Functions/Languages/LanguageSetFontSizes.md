# LanguageSetFontSizes

### Syntax

`LanguageSetFontSizes(language_id,size_array=[13,15,18,27,36,68])`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                                               |
| :----------- | :------- | :---------------------------------------------------------------------------- |
| langauge_id  | String   | The ID of the language you want to modify.                                    |
| size_array   | Array    | An array containing 6 real number entries. See the example provided down below. |

Modifies the font size for each step up in size. Zero Sievert has 6 font sizes it uses in various places. This allows you to configure the size of this font in each of those use cases, from smallest to largest.

### Example:

```
LanguageCreate("russian","Русский (Russian)","russian.csv","silver.ttf") 
LanguageSetFontSizes("russian",[13,15,18,27,36,68]) 
```

The above code will create a new language and configure the font sizes for each font size step.