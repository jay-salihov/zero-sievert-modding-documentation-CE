# Lexical Grammar

**Comments**
Not that there are no multi-line comments, instead write multiple comments.

```
-- This is a comment!
-- And this!
-- And this one too!
```

**Color Codes**

```
-- This is a pure white with RGB values (255,255,255)
#FFFFFF
```

**Strings**
There are two types of string literal in Catspeak. The most common is a sequence of characters starting and ending in double quotes (`"`):

```
let hi = "hello world"
```

This type of string allows the following escape sequences to be used:

*   `\"` Quotation mark
*   `\` Escape new line
*   `\\` Backslash
*   `\t` Character tabulation
*   `\n` Line feed
*   `\v` Line tabulation
*   `\f` Form feed
*   `\r` Carriage return

The other type of string is the **raw string**. Similarly to GML, a raw string is prefixed by the address symbol `@`, and does not interpret any of the previously mentioned escape sequences:

```
let hi_again = @"\hello\" -- \h and \" here are not escape sequences`
```

All strings in Catspeak can be multi-line.

**Keywords**
These are special identifiers which are reserved for use by Catspeak, and cannot be used as variables; Some of these have been modified from Catspeak's defaults, these are:

*   `true` Evaluates to boolean True.
*   `false` Evaluates to boolean False.
*   `undefined` GameMaker `undefined`.
*   `infinity` Floating-point positive infinity.
*   `NaN` Floating-point NaN.
*   `and` See [Logical Expressions](logical-expressions.md).
*   `or` See [Logical Expressions](logical-expressions.md).
*   `xor` See [Logical Expressions](logical-expressions.md).
*   `do` See [Block Expressions](block-expressions.md).
*   `if` See [If Expressions](if-expressions.md).
*   `else` See [If Expressions](if-expressions.md).
*   `while` See [While Expressions](while-expressions.md).
*   `with` See [With Expressions](with-expressions.md).
*   `match` See [Match Expressions](match-expressions.md).
*   `let` See [Let Statements](let-statements.md).
*   `func` See [Function Expressions](function-expressions.md).
*   `break` See [Break Expressions](break-expressions.md).
*   `continue` See [Continue Expressions](continue-expressions.md).
*   `return` See [Return Expressions](return-expressions.md).
*   `new` See [New Expressions](new-expressions.md).
*   `self` See [Self Expressions](self-expressions.md).