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
- The _Call Stack_ is the mechanism the JS interpreter uses to keep track of its place in a script that calls mutiple functions.
- JS is _single threaded_.

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
- ES6 introduces the _spread operator_ (`...`), which allows us to expand arrays and other expressions in places where multiple parameters or elements are expected.

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
| `.forEach()`  | Accepts a callback function. Calls the function once per element in the array.                                  |
| `.map()`      | Creates a new array with the results of calling a callback on every element in the array.                       |
| `.find()`     | Returns the value of the first element in the array that satisfies the provided testing function.               |
| `.filter()`   | Creates a new array with all elements that pass the test implemented by the provided function.                  |
| `.every()`    | Tests wether all elements in the array pass the provided function. It returns a Boolean value.                  |
| `.some()`     | Similar to every, but returns true if any of the array elements pass the test function.                         |
| `.reduce()`   | Executes a reducer function on each element of the array, resulting in a single value.                          |

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
- _Lexical scoper_ refers that inner functions within a function can access the variables declared.
- _Function Expressions_ is another way to declare functions:

  ```js
  const func = function () {
    // Code
  };
  ```

- _High Order Functions_ are functions that operate on/with other functions.
- _Callback Functions_ a callback function is a function passed into another function as an argument, which is invoked inside the outer function.
- _Hoisting_ takes functions to the top when compiled and you can declare them anywhere.
- ES6 provides us with the syntactic sugar to not have to write anonymous functions this way. Instead, you can use **arrow function syntax**:

  ```js
  const myFunc = () => {
    const myVar = 'value';
    return myVar;
  };
  ```

- In order to help us create more flexible functions, ES6 introduces _default parameters_ for functions.
- In order to help us create more flexible functions, ES6 introduces the _rest parameter_ for function parameters. With the rest parameter, you can create functions that take a variable number of arguments. These arguments are stored in an array that can be accessed later from inside the function.

  ```js
  function howMany(...args = 1) {
    return 'You have passed ' + args.length + ' arguments.';
  }
  ```

## Booleans

- Booleans may only be one of two values: `true` or `false`.

## If - Else

- `if` statements are used to make decisions in code. The keyword `if` tells JavaScript to execute the code in the curly braces under certain conditions, defined in the parentheses. These conditions are known as `Boolean` conditions and they may only be `true` or `false`.

  ```js
  if (condition is true) {
    //statement is executed
  }
  ```

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
- Another way to look for an specific key in a an object is by using the keryword `in`.
- When comparing objects you compare the reference and not the object properties, so they are never equal.
- `const` declaration alone doesn't really protect your data from mutation. To ensure your data doesn't change, JavaScript provides a function `Object.freeze` to prevent data mutation.
- _Destructuring assignment_ is special syntax introduced in ES6, for neatly assigning values taken directly from an object.
- Destructuring allows you to assign a new variable name when extracting values. You can do this by putting the new name after a colon when assigning the value.
- ES6 adds some nice support for easily defining _object literals_.

  ```js
  const getMousePosition = (x, y) => ({ x, y });
  ```

- With ES6, you can remove the function keyword and colon altogether when defining functions in objects. Here's an example of this syntax.

  ```js
  const person = {
    name: 'Taylor',
    sayHello() {
      return `Hello! My name is ${this.name}.`;
    },
  };
  ```

- ES6 provides a new syntax to create objects, using the class keyword.

  ```js
  class SpaceShuttle {
    constructor(targetPlanet) {
      this.targetPlanet = targetPlanet;
    }
  }
  const zeus = new SpaceShuttle('Jupiter');
  ```

- It should be noted that the `class` keyword declares a new function, to which a constructor is added. This constructor is invoked when `new` is called to create a new object.
- The `constructor` method is a special method for creating and initializing an object created with a class.
- **Getter** functions are meant to simply return (get) the value of an object's private variable to the user without the user directly accessing the private variable.
- **Setter** functions are meant to modify (set) the value of an object's private variable based on the value passed into the setter function. This change could involve calculations, or even overwriting the previous value completely.

  ```js
  class Book {
    constructor(author) {
      this._author = author;
    }
    // getter
    get writer() {
      return this._author;
    }
    // setter
    set writer(updatedAuthor) {
      this._author = updatedAuthor;
    }
  }
  ```

  - _this_ refers to the object that the method is associated with.
  - `instanceof` allows you to compare an object to a constructor, returning `true` or `false` based on whether or not that object was created with the constructor.
  - Properties in the _prototype_ are shared among ALL instances of the objects. Think of a _prototype_ as a "recipe" for creating objects.
  - All objects in JavaScript (with a few exceptions) have a _prototype_.
  - `Object` is a _supertype_ for all objects in JavaScript. Therefore, any object can use the `hasOwnProperty` method.
  - `Object.create(obj)` creates a new object, and sets `obj` as the new object's prototype.
  - Inheritance refers to adding the parent properties and methods to the child, you can use the keyword `extends` to extend a class.
  - `super`refers to the parent class constructor.
  - For unrelated objects, it's better to use _mixins_. A _mixin_ allows other objects to use a collection of functions.
  - The simplest way to make this public property private is by creating a variable within the constructor function. This changes the scope of that variable to be within the constructor function versus available globally. This way, the variable can only be accessed and changed by methods also within the constructor function.
  - In JavaScript, a function always has access to the context in which it was created. This is called `closure`.
  - A common pattern in JavaScript is to execute a function as soon as it is declared:

    ```js
    (function () {
      console.log('message');
    })();
    ```

- Note that the function has no name and is not stored in a variable. The two parentheses () at the end of the function expression cause it to be immediately executed or invoked. This pattern is known as an _immediately invoked function expression_ or _IIFE_.
- An immediately invoked function expression (IIFE) is often used to group related functionality into a single object or _module_.

## For - Each - While - Do While

- You can run the same code multiple times by using a loop.
- A `while` loop runs while a specified condition is `true` and stops once that condition is no longer `true`.
- The most common type of JavaScript loop is called a `for` loop because it runs for a specific number of times.
- `for (a; b; c)`, where a is the initialization statement, b is the condition statement, and c is the final expression.
- The condition statement is evaluated at the beginning of every loop iteration and will continue as long as it evaluates to `true`. When the condition is `false` at the start of the iteration, the loop will stop executing. This means if the condition starts as false, your loop will never execute.
- `do...while` loop will first do one pass of the code inside the loop no matter what, and then continue to run the loop `while` the specified condition evaluates to `true`.
- You can break out of a loop by using the keyword `break`;
- `For...of` for looping through _arrays_ in a more easy way.
- `For...in` for looping through _objects_ in a more easy way.

## Ternary Operator

- The _conditional operator_, also called the _ternary operator_, can be used as a one line if-else expression.
- The syntax is `a ? b : c`, where `a` is the condition, `b` is the code to run when the condition returns `true`, and `c` is the code to run when the condition returns `false`.

## Modules

- In order to make JavaScript more modular, clean, and maintainable; ES6 introduced a way to easily share code among JavaScript files. This involves exporting parts of a file for use in one or more other files, and importing the parts you need, where you need them. In order to take advantage of this functionality, you need to create a script in your HTML document with a `type` of `module`.

```js
<script type="module" src="filename.js"></script>
```

- A script that uses this `module` type can now use the `import` and `export` features you will learn about in the upcoming challenges.
- In order to share it with these other files, you first need to `export` it.

  ```js
  export const add = (x, y) => {
    return x + y;
  };
  ```

  ```js
  const add = (x, y) => {
    return x + y;
  };

  export { add };
  ```

- `import` allows you to choose which parts of a file or module to load.

  ```js
  import { add } from './math_functions.js';
  ```

  ```js
  import { add, subtract } from './math_functions.js';
  ```

- Suppose you have a file and you wish to import all of its contents into the current file. This can be done with the `import * as` syntax.

  ```js
  import * as myMathModule from './math_functions.js';
  ```

- There is another `export` syntax you need to know, known as _export default_. Usually you will use this syntax if only one value is being exported from a file. It is also used to create a fallback value for a file or module.
- To import a default export, you need to use a different `import` syntax.

  ```js
  import add from './math_functions.js';
  ```

## Promises

- A **promise** in JavaScript is exactly what it sounds like - you use it to make a promise to do something, usually asynchronously. When the task completes, you either fulfill your promise or fail to do so. `Promise` is a constructor function, so you need to use the `new` keyword to create one. It takes a function, as its argument, with two parameters - `resolve` and `reject`. These are methods used to determine the outcome of the promise.

```js
const myPromise = new Promise((resolve, reject) => {});
```

- A promise has three states: `pending`, `fulfilled`, and `rejected`.

```js
const myPromise = new Promise((resolve, reject) => {
  if(condition here) {
    resolve("Promise was fulfilled");
  } else {
    reject("Promise was rejected");
  }
});
```

- The `then` method is executed immediately after your promise is fulfilled with `resolve`.

```js
myPromise.then((result) => {});
```

- `catch` is the method used when your promise has been rejected.

  ```js
  myPromise.catch((error) => {});
  ```

- A _promise_ is an object representing the eventual completion or failure of an asynchronous operation.
- `new Promise((resolve, reject) => {});` where `resolve` is when the promise is successful and `reject` when the promise failed.
- `.then()` runs when the promise is resolved successfully.
- `.catch()` runs when the promise is rejected.
- You can chain the `.then()` for multiple requests.

## Regex

- Regular expressions are used in programming languages to match parts of strings. You create patterns to help you do that matching.
- JavaScript has multiple ways to use regexes. One way to test a regex is using the `.test()` method. The `.test()` method takes the **regex**, applies it to a string (which is placed inside the parentheses), and returns `true` or `false` if your pattern finds something or not.

  ```js
  let testStr = 'freeCodeCamp';
  let testRegex = /Code/;
  testRegex.test(testStr);
  ```

- This is powerful to search single strings, but it's limited to only one pattern. You can search for multiple patterns using the `alternation` or `OR` operator: `|`.
- This operator matches patterns either before or after it. For example, if you wanted to match the strings yes or no, the regex you want is `/yes|no/`.
- The flag that ignores case - the `i` flag.
- You can also extract the actual matches you found with the `.match()` method.
- To search or extract a pattern more than once, you can use the global search flag: `g`.
- The wildcard character `.` will match any one character.
- You can search for a literal pattern with some flexibility with _character classes_. Character classes allow you to define a group of characters you wish to match by placing them inside square (`[` and `]`) brackets.
- Inside a character set, you can define a range of characters to match using a hyphen character: `-`.
- To create a _negated character set_, you place a caret character (`^`) after the opening bracket and before the characters you do not want to match.
- Sometimes, you need to match a character (or group of characters) that appears one or more times in a row. This means it occurs at least once, and may be repeated. You can use the `+` character to check if that is the case.
- There's also an option that matches characters that occur zero or more times. The character to do this is the asterisk or star: `*`.
- In regular expressions, a _greedy_ match finds the longest possible part of a string that fits the regex pattern and returns it as a match. The alternative is called a _lazy_ match, which finds the smallest possible part of the string that satisfies the regex pattern.
- You can use the `?` character to change it to lazy matching.
- Outside of a character set, the caret (`^`) is used to search for patterns at the beginning of strings.
- You can search the end of strings using the dollar sign character `$` at the end of the regex.
- The closest character class in JavaScript to match the alphabet is `\w`. This shortcut is equal to `[A-Za-z0-9_]`. This character class matches upper and lowercase letters plus numbers.
- You can search for the opposite of the `\w` with `\W`. Note, the opposite pattern uses a capital letter. This shortcut is the same as `[^A-Za-z0-9_]`.
- The shortcut to look for digit characters is `\d`, with a lowercase d. This is equal to the character class `[0-9]`, which looks for a single character of any number between zero and nine.
- The shortcut to look for non-digit characters is `\D`. This is equal to the character class `[^0-9]`, which looks for a single character that is not a number between zero and nine.
- You can search for whitespace using `\s`, which is a lowercase `s`. This pattern not only matches whitespace, but also carriage return, tab, form feed, and new line characters.
- Search for non-whitespace using `\S`, which is an uppercase `s`. This pattern will not match whitespace, carriage return, tab, form feed, and new line characters.
- You can specify the lower and upper number of patterns with _quantity specifiers_. Quantity specifiers are used with curly brackets (`{` and `}`). You put two numbers between the curly brackets - for the lower and upper number of patterns.
- To only specify the lower number of patterns, keep the first number followed by a comma.
- To specify a certain number of patterns, just have that one number between the curly brackets.
- You can specify the possible existence of an element with a question mark, `?`. This checks for zero or one of the preceding element. You can think of this symbol as saying the previous element is optional.
- _Lookaheads_ are patterns that tell JavaScript to look-ahead in your string to check for patterns further along. This can be useful when you want to search for multiple patterns over the same string.
- There are two kinds of lookaheads: _positive lookahead_ and _negative lookahead_.
- A positive lookahead will look to make sure the element in the search pattern is there, but won't actually match it. A positive lookahead is used as `(?=...)` where the `...` is the required part that is not matched.
- On the other hand, a negative lookahead will look to make sure the element in the search pattern is not there. A negative lookahead is used as `(?!...)` where the `...` is the pattern that you do not want to be there. The rest of the pattern is returned if the negative lookahead part is not present.
- Sometimes we want to check for groups of characters using a Regular Expression and to achieve that we use parentheses `()`.
- Capture groups are constructed by enclosing the regex pattern to be captured in parentheses. In this case, the goal is to capture a word consisting of alphanumeric characters so the capture group will be `\w+` enclosed by parentheses: `/(\w+)/`.
- You can search and replace text in a string using `.replace()` on a string. The inputs for `.replace()` is first the regex pattern you want to search for. The second parameter is the string to replace the match or a function to do something.
- You can also access capture groups in the replacement string with dollar signs (`$`).

## Functional Programming

- Functional programming is a style of programming where solutions are simple, isolated functions, without any side effects outside of the function scope: `INPUT -> PROCESS -> OUTPUT`.
- Functional programming is about:
  1. Isolated functions - there is no dependence on the state of the program, which includes global variables that are subject to change.
  2. Pure functions - the same input always gives the same output.
  3. Functions with limited side effects - any changes, or mutations, to the state of the program outside the function are carefully controlled.
- Functions that can be assigned to a variable, passed into another function, or returned from another function just like any other normal value, are called _first class_ functions. In JavaScript, all functions are first class functions.
- The functions that take a function as an argument, or return a function as a return value are called _higher order_ functions.
- When functions are passed in to or returned from another function, then those functions which were passed in or returned can be called a _lambda_.
- Functional programming is a good habit. It keeps your code easy to manage, and saves you from sneaky bugs.
- Functional programming is a form of declarative programming. You tell the computer what you want done by calling a method or function.
- One of the core principles of functional programming is to not change things. Changes lead to bugs. It's easier to prevent bugs knowing that your functions don't change anything, including the function arguments or any global variable.
- Recall that in functional programming, changing or altering things is called _mutation_, and the outcome is called a _side effect_. A function, ideally, should be a _pure_ function, meaning that it does not cause any side effects.
- Another principle of functional programming is to always declare your dependencies explicitly. This means if a function depends on a variable or object being present, then pass that variable or object directly into the function as an argument.
- There are several good consequences from this principle. The function is easier to test, you know exactly what input it takes, and it won't depend on anything else in your program.
- This can give you more confidence when you alter, remove, or add new code. You would know what you can or cannot change and you can see where the potential traps are.
- Finally, the function would always produce the same output for the same set of inputs, no matter what part of the code executes it.
- It would make sense to be able to pass them as arguments to other functions, and return a function from another function. Functions are considered _first class objects_ in JavaScript, which means they can be used like any other object. They can be saved in variables, stored in an object, or passed as function arguments.
- Functional programming is all about creating and using non-mutating functions.
- The _arity_ of a function is the number of arguments it requires. _Currying_ a function means to convert a function of N arity into N functions of arity 1.
- Similarly, _partial application_ can be described as applying a few arguments to a function at a time and returning another function that is applied to more arguments.

## Debug

- The `console.log()` method, which "prints" the output of what's within its parentheses to the console, will likely be the most helpful debugging tool. Placing it at strategic points in your code can show you the intermediate values of variables.
- You can use `typeof` to check the data structure, or type, of a variable.
- _Off by one errors_ (sometimes called OBOE) crop up when you're trying to target a specific index of a string or array (to slice or access a segment), or when looping over the indices of them. JavaScript indexing starts at zero, not one, which means the last index is always one less than the length of the item. If you try to access an index equal to the length, the program may throw an "index out of range" reference error or print `undefined`.

## Data Structures

- In Computer Science a **queu** is an abstract _Data Structure_ where items are kept in order. New items can be added at the back of the queue and old items are taken off from the front of the queue.
- Recursion is the concept that a function can be expressed in terms of itself.

## DOM

- The Document Object Model (DOM) is a representation of a webpage.
- The _document_ is the entry point to all the DOM.
- `document.getElementById()` gets the element by the id given in the html attributes.
- `document.getElementsByTagName()` gets all elements with the given tag, you can manipulate this elements by using some array methods.
- `document.getElementByClassName()` or `document.getElementsByClassName()` gets all elements with the given class, you can manipulate this elements by using some array methods.
- `document.querySelector()` or `document.querySelectorAll()` gets all elements with the given CSS selector, you can manipulate this elements by using some array methods.
- `.innerText` displays the text inside an element and let you change its contents.
- `.textContent` displays the text inside an element keeping the original format and let you change its contents.
- `.innerHTML` displays the HTML content of the selected element.
- `.value` or `.checked` checks the value assigned to an input.
- `.getAttribute` gets the specified attribute value.
- `.setAttribute` sets the specified attribute to the new specified values.
- `.parentElement` gets the parent element of the selected element.
- `.children` gets the children element of the selected element.
- `nextElementSibling` gets the next element of the selected element.
- `previousElementSibling` gets the previous element of the selected element.
- `.style.<property>` changes the CSS style for the selected element.
- `getComputedStyle` gets all the CSS computed styles for the selected element.
- `.classList` lets you manipulate classes like adding or removing to the selected element.
- `.createElement` creates the specified HTML element.
- `.appendChild` appends to the DOM the created element.
- `.insertBefore` appends element at the beggining of the specified element.
- `.insertAdjacentElement` appends element to the specified position of the specified element.
- `.append` appends to the end of the selected element.
- `.prepend` appends to the beggining of the selected element.
- `.remove` removes the selected element.
- `.addEventListener` adds an event listener to an action for the element. It also recieves an event that can be accessed in the function, this event can be used to check for different events.
- `event.preventDefault()` prevents the default behaivor when sending a form through JS.
- When using a form it's better to recieve the inputs by name using the _input_ event listener and asign them to a object.

## HTTP Requests

- _AJAX_ = Asynchronous Javascript and XML.
- _JSON_ = Javascript Object Notation.
- _Fetch API_ = Newer way of making requests via JS using promises.

  ```js
  fetch('url').then((response) => {
    console.log(response.json());
  });
  ```

- To throw an error you can use `throw new Error()`.
- You can chain multiple requests using _promises_.
- _Axios_ = A library for making HTTP request (more easy than fetch API).

## Async Functions

- Syntactic sugar for promises, but works the same as promises.
- Async functions always return promises.
- `async` for declaring a function asyncronous.
- `await` for waiting the response.
- You can _catch_ errors in an async function by using `try` and `catch`.
- You can chain multiple `await` for multiple requests.
- You can use `Promise.all([])` to wait for all the promises to resolve.
  -s
