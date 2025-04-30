# Expressions

There are various expressions used for loops, building anonymous functions, and more.
There is a bit more information that you can find [here](), however some of the keywords may not match the keywords used within the Zero Sievert modding system.

**Functions**

```
let this_is_a_function = func(b) {
  -- We can put code in here
  let a = 0;
  return a + b;
}

this_is_a_function()
```

**Arrays**

```
let array = [1, 2, 3]

array[0] = 5;
array[1] = 10;
array[2] = 15;
```

**Structs**

```
let struct = { x : 0, y : 0}

struct.x = 5;
struct.y = 10;
```

**With**

```
let struct = { x : 0 }

with ( struct ) {
  x += 5;
}
```

**While**

```
-- Example 1
let a = 0;

while ( a < 10 ) {
  a += 1;
}
```

```
-- Example 2
let a = 0;

while ( true ) {
  a += 1;

  if ( a > 10 ) {
    break;
  }
}
```

**Match (Switch)**

```
let color

match player {
  case "Dave" {
    colour = #e00707
  }
  case "Rose" {
    colour = #b536da
  }
  case "Dash" {
    colour = #f2a400
  }
  case "Roxy" {
    colour = #ff6ff2
  }
  else {
    show_message("invalid player")
  }
}
```