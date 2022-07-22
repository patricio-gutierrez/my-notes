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
- In order to get the last letter of a string, you can subtract one from the string's length.

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

## Arrays

- With JavaScript `array` variables, we can store several pieces of data in one place.
- You can also nest arrays within other arrays. This is also called a _multi-dimensional_ array.
- We can access the data inside arrays using _indexes_.
- Array indexes are written in the same bracket notation that strings use, except that instead of specifying a character, they are specifying an entry in the array. Like strings, arrays use zero-based indexing, so the first element in an array has an index of `0`.
- Unlike strings, the entries of arrays are _mutable_ and can be changed freely, even if the array was declared with `const`.
- One way to think of a _multi-dimensional array_, is as an _array of arrays_. When you use brackets to access your array, the first set of brackets refers to the entries in the outer-most (the first level) array, and each additional pair of brackets refers to the next level of entries inside.

| Method        | Description                                                                                                     |
| ------------- | --------------------------------------------------------------------------------------------------------------- |
| `.push()`     | Append a value to the **end** of an array.                                                                      |
| `.pop()`      | Pop a value of the **end** of an array. We can store this popped off value by assigning it to a variable.       |
| `.shift()`    | Pop a value of the **beginning** of an array. We can store this popped off value by assigning it to a variable. |
| `.unshift()`  | Append a value to the **beginning** of an array.                                                                |
| `.concat()`   | Appends one array with another.                                                                                 |
| `.includes()` | Searches for a value in the array and returns true or false.                                                    |
| `.indexOf()`  | Searches for a value in the array and return the position.                                                      |
| `.reverse()`  | Reverses an array.                                                                                              |
| `.join()`     | Joins an array and converts it into a string.                                                                   |
| `.slice()`    | Copy a portion of an array.                                                                                     |
| `.splice()`   | Remove/replace elements of an array.                                                                            |
| `.sort()`     | Sort elements of an array.                                                                                      |

## Functions

- In JavaScript, we can divide up our code into reusable parts called _functions_.

  ```js
  function functionName() {
    console.log('Hello World');
  }
  ```

- You can call or invoke this function by using its name followed by parentheses, like this: `functionName();`.
- _Parameters_ are variables that act as placeholders for the values that are to be input to a function when it is called. When a function is defined, it is typically defined along with one or more parameters. The actual values that are input (or _"passed"_) into a function when it is called are known as _arguments_.

  ```js
  function testFun(param1, param2) {
    console.log(param1, param2);
  }
  ```

- You can use a `return` statement to send a value back out of a function.
- In JavaScript, **scope** refers to the visibility of variables. Variables which are defined outside of a function block have _Global_ scope. This means, they can be seen everywhere in your JavaScript code.
- Variables which are declared within a function, as well as the function parameters, have _local_ scope. That means they are only visible within that function.
- It is possible to have both _local_ and _global_ variables with the same name. When you do this, the local variable takes precedence over the global variable.
- A function can include the `return` statement but it does not have to. In the case that the function doesn't have a `return` statement, when you call it, the function processes the inner code but the returned value is `undefined`.

## Booleans

- Booleans may only be one of two values: `true` or `false`.

## If - Else

- `if` statements are used to make decisions in code. The keyword `if` tells JavaScript to execute the code in the curly braces under certain conditions, defined in the parentheses. These conditions are known as `Boolean` conditions and they may only be `true` or `false`.
- When the condition evaluates to `true`, the program executes the statement inside the curly braces. When the Boolean condition evaluates to `false`, the statement inside the curly braces will not execute.
- The most basic operator is the equality operator `==`. The equality operator compares two values and returns `true` if they're equivalent or `false` if they are not.
- Strict equality (`===`), if the values being compared have different types, they are considered unequal, and the strict equality operator will return false.
- The inequality operator (`!=`) is the opposite of the equality operator. It means not equal and returns `false` where equality would return `true` and vice versa.
- The strict inequality operator (`!==`) is the logical opposite of the strict equality operator. It means "Strictly Not Equal" and returns `false` where strict equality would return `true` and vice versa. The strict inequality operator **will not convert data types**.
- The greater than operator (`>`) compares the values of two numbers. If the number to the left is greater than the number to the right, it returns `true`. Otherwise, it returns `false`.
- The greater than or equal to operator (`>=`) compares the values of two numbers. If the number to the left is greater than or equal to the number to the right, it returns `true`. Otherwise, it returns `false`.
- The less than operator (`<`) compares the values of two numbers.
- The less than or equal to operator (`<=`) compares the values of two numbers.
- Sometimes you will need to test more than one thing at a time. The logical and operator (`&&`) returns `true` if and only if the operands to the left and right of it are `true`.
- The logical or operator (`||`) returns `true` if either of the operands is true. Otherwise, it returns `false`.
- With an `else` statement, an alternate block of code can be executed whe the code is `false`.
- If you have multiple conditions that need to be addressed, you can chain `if` statements together with `else if` statements.

  ```js
  if (condition1) {
    statement1
  } else if (condition2) {
    statement2
  } else if (condition3) {
    statement3
  . . .
  } else {
    statementN
  }
  ```

## Switch

- A `switch` statement tests a value and can have many case statements which define various possible values. Statements are executed from the first matched `case` value until a `break` is encountered.
- In a `switch` statement you may not be able to specify all possible values as `case` statements. Instead, you can add the `default` statement which will be executed if no matching `case` statements are found.
- If the `break` statement is omitted from a `switch` statement's `case`, the following `case` statement(s) are executed until a `break` is encountered.

  ```js
  switch (lowercaseLetter) {
    case 'a':
      console.log('A');
      break;
    case 'b':
      console.log('B');
      break;
    default:
      defaultStatement;
      break;
  }
  ```

## Objects

- Objects are similar to `arrays`, except that instead of using indexes to access and modify their data, you access the data in objects through what are called `properties`.
- Objects are useful for storing data in a structured way, and can represent real world objects.

  ```js
  const cat = {
    name: 'Whiskers',
    legs: 4,
    tails: 1,
    enemies: ['Water', 'Dogs'],
  };
  ```

- There are two ways to access the properties of an object: dot notation (`.`) and bracket notation (`[]`), similar to an array.
- Another use of bracket notation on objects is to access a property which is stored as the value of a variable. This can be very useful for iterating through an object's properties or when accessing a lookup table.
- We can also delete properties from objects using the keyword `delete`.
- Objects can be thought of as a **key/value storage**, like a dictionary. If you have tabular data, you can use an object to lookup values.
- Sometimes it is useful to check if the property of a given object exists or not. We can use the `.hasOwnProperty(propname)` method of objects to determine if that object has the given property name.
- When comparing objects you compare the reference and not the object properties, so they are never equal.

## For - Each - While - Do While

- You can run the same code multiple times by using a loop.
- A `while` loop runs while a specified condition is `true` and stops once that condition is no longer `true`.
- The most common type of JavaScript loop is called a `for` loop because it runs for a specific number of times.
- `for (a; b; c)`, where a is the initialization statement, b is the condition statement, and c is the final expression.
- The condition statement is evaluated at the beginning of every loop iteration and will continue as long as it evaluates to `true`. When the condition is `false` at the start of the iteration, the loop will stop executing. This means if the condition starts as false, your loop will never execute.
- `do...while` loop will first do one pass of the code inside the loop no matter what, and then continue to run the loop `while` the specified condition evaluates to `true`.

## Ternary Operator

- The _conditional operator_, also called the _ternary operator_, can be used as a one line if-else expression.
- The syntax is `a ? b : c`, where `a` is the condition, `b` is the code to run when the condition returns `true`, and `c` is the code to run when the condition returns `false`.

## Data Structures

- In Computer Science a **queu** is an abstract _Data Structure_ where items are kept in order. New items can be added at the back of the queue and old items are taken off from the front of the queue.

  ```js
  if (condition is true) {
    //statement is executed
  }
  ```

- Recursion is the concept that a function can be expressed in terms of itself.
