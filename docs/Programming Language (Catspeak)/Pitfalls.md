# Pitfalls

Some of this section is copied from the official catspeak documentation.

Catspeak is **not** GML, and so you should not assume it will behave identically to GML. This section lists the common differences between GML and the Catspeak programming language:

**Variables**:

*   Local variables in Catspeak are **declared using `let`**, not `var`. (See [Let Statements](let-statements.md))
*   Local variables and function definitions are **not [hoisted](https://en.wikipedia.org/wiki/Hoisting_(programming))**; that is, *using local variables and functions before they are defined*. (See [Let Statements](let-statements.md) and [Function Expressions](function-expressions.md))

```
 show_mesage(my_var) -- does NOT print '2'
 let my_var = 2
```

*   To access instance variables you need to **explicitly write `self`**. (See [Self Expressions](self-expressions.md))To access instance variables you need to **explicitly write `self`**. (See [Self Expressions](self-expressions.md))

```
let a = item -- 'item' refers to a Catspeak variable here
let b = self.item -- 'item' refers to a GML instance variable here
```

*   **Syntax**:

    *   `++` and `--` are **not valid operators** use `i += 1` and `i -= 1` instead. (See [Operators](operators.md))
    *   Catspeak reserves `--` **for comments**. (See [Operators](operators.md) and [Comments](comments.md))
    *   Catspeak reserves `//` for **integer division**. (See [Operators](operators.md) and [Comments](comments.md))
    *   The ternary operator `condition ? a : b` **does not exist** in Catspeak, instead the [If Expression](if-expressions.md) should be used `if a > b { a } else { b }`
    *   **`for`**, **`repeat`**, and **`do` loops do not exist**. Instead you should use [While Loops](while-loops.md).
    *   **`switch` does not exist**. Instead you should use [Match Expressions](match-expressions.md).
    *   There are **no `[@` and `[$` accessors**, both structs and arrays can be indexed using `a[i]`. (See [Accessor Expressions](accessor-expressions.md))
    *   There are **no `[#`, `[?`, and `[|` accessors**. Data structures should use functions like `ds_list_get` and `ds_list_set`, if exposed by the modding API.