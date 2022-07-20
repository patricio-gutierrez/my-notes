# Javascript Concepts

## Basics

- Comments are lines of code that JavaScript will intentionally ignore. Comments are a great way to leave notes to yourself and to other people who will later need to figure out what that code does.
  - `// This is a comment`
  - `/* This is a multiline comment */`
- JS offers 8 different _data types_:
  - `undefined`
  - `null`
  - `boolean`
  - `string`
  - `symbol`
  - `bigint`
  - `number`
  - `object`
- _Variables_ allow computers to store and manipulate data in a dynamic fashion. They do this by using a "label" to point to the data rather than using the data itself.
- In JavaScript, you can store a value in a variable with the _assignment_ operator (`=`).
- It is common to _initialize_ a variable to an initial value in the same line as it is declared.
- A _string literal_, or _string_, is a series of zero or more characters enclosed in single or double quotes.
- When JavaScript variables are declared, they have an initial value of `undefined`.
- If you do a mathematical operation on an `undefined` variable your result will be `NaN` which means _"Not a Number"_.
- In JavaScript all variables and function names are case sensitive. This means that capitalization matters.
- In _camelCase_, multi-word variable names have the first word in lowercase and the first letter of each subsequent word is capitalized.
- A keyword called `let` was introduced in ES6, a major update to JavaScript, to solve this potential issue with the `var` keyword.
- `const` has all the awesome features that `let` has, with the added bonus that variables declared using `const` are read-only. They are a constant value, which means that once a variable is assigned with `const`, it cannot be reassigned.
- You can easily _increment_ or add one to a variable with the `++` operator.
- You can easily _decrement_ or decrease a variable by one with the `--` operator.
- We can store decimal numbers in variables too. Decimal numbers are sometimes referred to as _floating point numbers_ or _floats_.
- The _remainder_ operator `%` gives the remainder of the division of two numbers.
- In JavaScript, you can _escape_ a quote from considering it as an end of string quote by placing a _backslash_ (`\`) in front of the quote.
- _String_ values in JavaScript may be written with single or double quotes, as long as you start and end with the same type of quote.
- In JavaScript, when the `+` operator is used with a `String` value, it is called the _concatenation_ operator. You can build a new string out of other strings by _concatenating_ them together.
- We can also use the `+=` operator to _concatenate_ a string onto the end of an existing string variable. This can be very helpful to break a long string over several lines.
- You can find the length of a `String` value by writing `.length` after the string variable or string literal.
- _Bracket notation_ is a way to get a character at a specific index within a string.
- Most modern programming languages, like JavaScript, don't start counting at 1 like humans do. They start at 0. This is referred to as _Zero-based_ indexing.
- In JavaScript, String values are _immutable_, which means that they cannot be altered once created.
- String template literals are strings that allow embedded expressions enclosed in ``.
- `typof` gives you the type of a value.
- `parseInt()` & `parseFloat()` parse strings into numbers.

## String Methods

| Method              | Description                                |
| ------------------- | ------------------------------------------ |
| `.length`           | Length of the string.                      |
| `.toUpperCase()`    | Uppercases the string.                     |
| `.toLowerCase()`    | Lowercases the string.                     |
| `.trim()`           | Trims spaces in the string.                |
| `.indexOf(string)`  | Returns the index where the word is found. |
| `.slice(beggining)` | Slices from beggining index to the end.    |
| `.replace(string)`  | Replaces the string wiht the string given. |

## Data Types

| Type        | Description                                       |
| ----------- | ------------------------------------------------- |
| `Number`    | Numeric data.                                     |
| `Boolean`   | `true` or `false` values only.                    |
| `String`    | Strings of characters.                            |
| `Null`      | Intentional absence of a value. Must be assigned. |
| `Undefined` | Variable that does not have an assigned value.    |
