<!--
link: styles.css
-->

# Nodejs

## ES 6 Features for Node

### ECMAScript

**History**

ECMAScript is based on several originating technologies, the most well-known being JavaScript (Netscape) and JScript (Microsoft). The language was invented by `Brendan Eich` at `Netscape` and first appeared in that company's `Navigator 2.0 browser`. It has appeared in all subsequent browsers from Netscape and in all browsers from `Microsoft` starting with `Internet Explorer 3.0`.

![Ecma International Logo](./images/ecmascript/ecma-logo.svg "Ecma International Logo")

Netscape called it `Javascript` just for marketing because `java` was popular back then. Then microsoft came up with their language `JScript` to add interactivity to their browser `Internet Explorer`. Without any standards it was hard on developers to create websites that worked well in both leading browsers of that time. Netscape approached [`Ecma International`](https://www.ecma-international.org/) to set a standard. Ecma International is an organisation that sets technology standards. Oracle owns the trademark of Javascript, so Ecma International called it ECMAScript. Specification is called ECMA-262, it's like a catalogue number among other standards that are maintained by Ecma International.

This Ecma Standard defines the ECMAScript 2023 Language. It is the fourteenth edition of the ECMAScript Language Specification. Since publication of the first edition in 1997, ECMAScript has grown to be one of the world's most widely used general-purpose programming languages. It is best known as the language embedded in web browsers but has also been widely adopted for server and embedded applications.

The development of the ECMAScript Language Specification started in November 1996. The first edition of this Ecma Standard was adopted by the Ecma General Assembly of June 1997. From then on multiple ECMA-262 editions were launched. Each with a new enhancements. ES6 or ES2015 was the 6th edition and was released in 2015. Post that each years release has been called by the year. Example ES2016, ES2017 etc.

The third edition of the Standard introduced powerful regular expressions, better string handling, new control statements, try/catch exception handling, tighter definition of errors, formatting for numeric output and minor changes in anticipation of future language growth. The third edition of the ECMAScript standard was adopted by the Ecma General Assembly of December 1999 and published as ISO/IEC 16262:2002 in June 2002.

After publication of the third edition, ECMAScript achieved massive adoption in conjunction with the World Wide Web where it has become the programming language that is supported by essentially all web browsers. Significant work was done to develop a fourth edition of ECMAScript. However, that work was not completed and not published as the fourth edition of ECMAScript but some of it was incorporated into the development of the sixth edition.

The fifth edition of ECMAScript (published as ECMA-262 5th edition) codified de facto interpretations of the language specification that have become common among browser implementations and added support for new features that had emerged since the publication of the third edition. Such features include accessor properties, reflective creation and inspection of objects, program control of property attributes, additional array manipulation functions, support for the JSON object encoding format, and a strict mode that provides enhanced error checking and program security. The fifth edition was adopted by the Ecma General Assembly of December 2009.

The fifth edition was submitted to ISO/IEC JTC 1 for adoption under the fast-track procedure, and approved as international standard ISO/IEC 16262:2011. Edition 5.1 of the ECMAScript Standard incorporated minor corrections and is the same text as ISO/IEC 16262:2011. The 5.1 Edition was adopted by the Ecma General Assembly of June 2011.

Focused development of the sixth edition started in 2009, as the fifth edition was being prepared for publication. However, this was preceded by significant experimentation and language enhancement design efforts dating to the publication of the third edition in 1999. In a very real sense, the completion of the sixth edition is the culmination of a fifteen year effort. The goals for this edition included providing better support for large applications, library creation, and for use of ECMAScript as a compilation target for other languages. Some of its major enhancements included modules, class declarations, lexical block scoping, iterators and generators, promises for asynchronous programming, destructuring patterns, and proper tail calls. The ECMAScript library of built-ins was expanded to support additional data abstractions including maps, sets, and arrays of binary numeric values as well as additional support for Unicode supplementary characters in strings and regular expressions. The built-ins were also made extensible via subclassing. The sixth edition provides the foundation for regular, incremental language and library enhancements. The sixth edition was adopted by the General Assembly of June 2015.

ECMAScript 2016 was the first ECMAScript edition released under Ecma TC39's new yearly release cadence and open development process. A plain-text source document was built from the ECMAScript 2015 source document to serve as the base for further development entirely on GitHub. Over the year of this standard's development, hundreds of pull requests and issues were filed representing thousands of bug fixes, editorial fixes and other improvements. Additionally, numerous software tools were developed to aid in this effort including Ecmarkup, Ecmarkdown, and Grammarkdown. ES2016 also included support for a new exponentiation operator and adds a new method to Array.prototype called includes.

ECMAScript 2017 introduced Async Functions, Shared Memory, and Atomics along with smaller language and library enhancements, bug fixes, and editorial updates. Async functions improve the asynchronous programming experience by providing syntax for promise-returning functions. Shared Memory and Atomics introduce a new memory model that allows multi-agent programs to communicate using atomic operations that ensure a well-defined execution order even on parallel CPUs. It also included new static methods on Object: Object.values, Object.entries, and Object.getOwnPropertyDescriptors.

ECMAScript 2018 introduced support for asynchronous iteration via the AsyncIterator protocol and async generators. It also included four new regular expression features: the dotAll flag, named capture groups, Unicode property escapes, and look-behind assertions. Lastly it included object rest and spread properties.

ECMAScript 2019 introduced a few new built-in functions: flat and flatMap on Array.prototype for flattening arrays, Object.fromEntries for directly turning the return value of Object.entries into a new Object, and trimStart and trimEnd on String.prototype as better-named alternatives to the widely implemented but non-standard String.prototype.trimLeft and trimRight built-ins. In addition, it included a few minor updates to syntax and semantics. Updated syntax included optional catch binding parameters and allowing U+2028 (LINE SEPARATOR) and U+2029 (PARAGRAPH SEPARATOR) in string literals to align with JSON. Other updates included requiring that Array.prototype.sort be a stable sort, requiring that JSON.stringify return well-formed UTF-8 regardless of input, and clarifying Function.prototype.toString by requiring that it either return the corresponding original source text or a standard placeholder.

ECMAScript 2020, the 11th edition, introduced the matchAll method for Strings, to produce an iterator for all match objects generated by a global regular expression; import(), a syntax to asynchronously import Modules with a dynamic specifier; BigInt, a new number primitive for working with arbitrary precision integers; Promise.allSettled, a new Promise combinator that does not short-circuit; globalThis, a universal way to access the global this value; dedicated export \* as ns from 'module' syntax for use within modules; increased standardization of for-in enumeration order; import.meta, a host-populated object available in Modules that may contain contextual information about the Module; as well as adding two new syntax features to improve working with “nullish” values (null or undefined): nullish coalescing, a value selection operator; and optional chaining, a property access and function invocation operator that short-circuits if the value to access/invoke is nullish.

ECMAScript 2021, the 12th edition, introduced the replaceAll method for Strings; Promise.any, a Promise combinator that short-circuits when an input value is fulfilled; AggregateError, a new Error type to represent multiple errors at once; logical assignment operators (??=, &&=, ||=); WeakRef, for referring to a target object without preserving it from garbage collection, and FinalizationRegistry, to manage registration and unregistration of cleanup operations performed when target objects are garbage collected; separators for numeric literals (1_000); and Array.prototype.sort was made more precise, reducing the amount of cases that result in an implementation-defined sort order.

ECMAScript 2022, the 13th edition, introduced top-level await, allowing the keyword to be used at the top level of modules; new class elements: public and private instance fields, public and private static fields, private instance methods and accessors, and private static methods and accessors; static blocks inside classes, to perform per-class evaluation initialization; the #x in obj syntax, to test for presence of private fields on objects; regular expression match indices via the /d flag, which provides start and end indices for matched substrings; the cause property on Error objects, which can be used to record a causation chain in errors; the at method for Strings, Arrays, and TypedArrays, which allows relative indexing; and Object.hasOwn, a convenient alternative to Object.prototype.hasOwnProperty.

ECMAScript 2023, the 14th edition, introduced the toSorted, toReversed, with, findLast, and findLastIndex methods on Array.prototype and TypedArray.prototype, as well as the toSpliced method on Array.prototype; added support for #! comments at the beginning of files to better facilitate executable ECMAScript files; and allowed the use of most Symbols as keys in weak collections.

### Babel Transpiler

[Babel](https://babeljs.io/) is a toolchain that is mainly used to convert ECMAScript 2015+ code into a backwards compatible version of JavaScript in current and older browsers or environments. Basically, it allows us to write Javascript code using its latest features and not worry about it working in older browsers or environements which do not yet support those features.

> **Compiler** A compiler is a tool that takes source code written in one programming language and translates it into another language, typically a lower-level language or machine code.
>
> **Tranpiler** A transpiler, short for "source-to-source compiler," is a specific type of compiler that translates source code from one high-level programming language to another high-level programming language. In the context of Babel, it does involve source-to-source transformation because it converts one form of JavaScript source code to another form of JavaScript source code.

Lets see an example of what babel does.

**Javascript code with ES6 features**

```javascript
const sayHello = (name) => {
  let message = `Hello, ${name}!`;
  console.log(message);
};

sayHello("World");
```

**Javascript code transpiled to ES5**

```javascript
"use strict";

var sayHello = function sayHello(name) {
  var message = "Hello, ".concat(name, "!");
  console.log(message);
};
sayHello("World");
```

Babel transpiled Arrow functions and string literal syntaxes into ES5 sytaxes which are supported by most of the browsers.

**Configuring Babel**

- Initialise a node project by running the comamnd `npm init -y`.
- Run the command `npm install --save-dev @babel/core @babel/cli @babel/preset-env` to install babel as dev dependency.
- Create a file `index.js` where our code goes.
- Create a `.babelrc` file to add babel configurations.
- Add below json into babelrc file. `presets` say what all syntaxes to convert to older version of js. [`@babel/preset-env`](https://babeljs.io/docs/babel-preset-env) sets all the default conversions required.

```json
{
  "presets": ["@babel/preset-env"]
}
```

- Add scripts to build and in `package.json` file.

```json
"scripts": {
    "build": "babel index.js -d dist",
    "start": "node dist/index.js"
}
```

- `npm run build` will tranpile the contents of `index.js` file and place it into `dist/index.js`.
- `npm start` will run the `dist/index.js` file.

### Let, Const and Block scope

**Let Keyword**

1. _Variables defined with let cannot be Redeclared._

```javascript
let number = 5;
let number = 10;
```

This will throw <div class="color-red">SyntaxError: Identifier 'number' has already been declared</div>

Variables declared with `let` cannot be redeclared. But variables declared with `var` can be redeclared.

```javascript
var number = 5;
var number = 10;
```

This will not throw any error.

2. _Variables defined with let must be Declared before use._

```javascript
let total = number + number;
console.log(total);
let number = 5;
```

This will throw <div class="color-red">ReferenceError: Cannot access 'number' before initialization</div>

`var` allows such behaviour. Variable will be assigned the value `undefined` before initialisation. This is called as Hoisting.

```javascript
var total = number + number;
console.log(total); // Nan
var number = 5;
```

This will not throw any error. It'll log `NaN` to console as `undefined + undefined = Nan`.

3. _Variables defined with let have Block Scope._

```javascript
if (true) {
  let number = 5;
}
console.log(number);
```

This will throw <div class="color-red">ReferenceError: number is not defined</div>

```javascript
if (true) {
  var number = 5;
}
console.log(number); // 5
```

This will not throw any error. It'll log `5` to the console as `var` keyword is `function scoped`.

**Const Keyword**

1. _Variables defined with const cannot be Redeclared._
2. _Variables defined with const have Block Scope._
   Above 2 statements are similar to how `let` behaves.

3. _Variables defined with const must be Initialised._

```javascript
const number;
number = 5;
console.log(number);
```

This will throw <div class="color-red">SyntaxError: Missing initializer in const declaration</div>

```javascript
let number;
number = 5;
console.log(number); // 5
```

This will not throw any error. Variable with `let` keyword can be defined and then initialised which is not the case with `const`

4. _Variables defined with const cannot be Reassigned._

```javascript
const number;
number = 5;
console.log(number);
```

This will throw <div class="color-red">TypeError: Assignment to constant variable.</div>

```javascript
let number;
number = 5;
console.log(number); // 5
```

This will not throw any error. Variable with `let` keyword can be reassigned.

### String template literals

String literals are defined using `\`(back tick)` instead of single or double quotes.

```javascript
const string1 = `Hello world`;
const string2 = `I'll learn "Javascript"`;
const string3 = `I'll learn "Javscript"
then learn "Python"`;

console.log(string1);
console.log(string2);
console.log(string3);
```

Output

```javascript +@output
Hello world
I'll learn "Javascript"
I'll learn "Javscript"
then learn "Python"
```

It's very convenient to add quotes in string using back ticks. It also retains multiline string formatting. We don't have to add new line character to jump line anymore.

World without template literals would be.

```javascript
const string1 = "Hello world";
const string2 = 'I\'ll learn "Javascript"';
const string3 = 'I\'ll learn "Javscript"\nthen learn "Python"';
```

Template literals also make string interpolation easy. Using `${}` we can add variable or expression between a string. Let's see few examples of how we can do string interpolation.

Example

```javascript
const first = "Hello";
const last = "World";
const string = `${first}, ${last}!`;
console.log(string); // Hello, World!
```

Example

```javascript
const number = -1;
console.log(`Number is ${number > 0 ? "Positive" : "Negative"}`); // Number is Negative
```

Example

```javascript
const isPositive = (number) => (number > 0 ? "Positive" : "Negative");
const number = 5;
console.log(`Number is ${isPositive()}`); // Number is Positive
```

### Arrow Functions

Arrow functions are a way to write functions in a consice form without using the keyword `function`.

```javascript
//Regular function with function keyword
function sayHello() {
  console.log("Hello World");
}

//Arrow function
const sayHello = () => {
  console.log("Hello World");
};
```

Few key points to note:-

1. Arrow functions don't have their own bindings to `this`, `arguments`, or `super`, and should not be used as `methods`.
2. Arrow functions cannot be used as `constructors`. Calling them with `new` throws a `TypeError`.

Let's see how we can write Arrow functions in different scenarios.

```javascript
// Regular function which returns the square of a number
function square(num) {
  return num * num;
}

// Arrow function with function keyword removed
const square = (num) => {
  return num * num;
};

// Brackets and return keyword can be removed if there is a single statement in function body
const square = (num) => num * num;

// Paranthesis around argument can be removed if its single
const square = (num) => num * num;
```

Returning an Object literal without return statement will throw an error.

```javascript
// Throws error
const getLanguageInfo = () => {name: "Javascript", version: "ES6"};

// Enclose Object with Paranthesis for it work
const getLanguageInfo = () => ({name: "Javascript", version: "ES6"});
```

**This keyword**

`this` keyword behaves differently with Regular functions and Arrow functions. In Regular function `this` refers to the object which called the function. Arrow functions do not have their own `this` binding and instead `inherit` it from it's lexical context.

In Node environment, `this` within Regular function refers to `global` and outside it refers to `module.exports`. Within a method part of an object refers to the object.

```javascript
// this accessed outside a function
console.log(module.exports === this); // true

// this accessed inside a function
(function sayHello() {
  console.log(global === this); //true
})();

// this refers to the language object
const language = {
  name: "Javascript",
  version: "ES6",
  getInfo: function () {
    console.log(module.exports === this); // false
    console.log(global === this); // false
    console.log(this.name); // Javascript
  },
};
language.getInfo();
```

> Self calling function syntax from above is called `Immediately Invoked Function Expression(IIFE)`.

```javascript
// this keyword refers to its lexical context's this. i.e global
const language = {
  name: "Javascript",
  version: "ES6",
  getInfo: () => {
    console.log(module.exports === this); // false
    console.log(global === this); // true
    console.log(this.name); // undefined
  },
};
language.getInfo();

// second this keyword inside IIFE points to its parent's scope. ie. language object.
const language = {
  name: "Javascript",
  version: "ES6",
  getInfo: function () {
    console.log(module.exports === this); // false
    console.log(global === this); // true
    console.log(this); // undefined
    (() => {
      console.log(module.exports === this); // false
      console.log(global === this); // false
      console.log(this); // Javascript
    })();
  },
};

language.getInfo();
```

> Above code snippet shows why Arrow functions should not be used for methods as this doesn't point to the object.

Arrow functions cannot be used as the `super` keyword because arrow functions do not have their own super binding. The super keyword is used to call methods on an object's parent class (i.e., in the context of inheritance and class constructors).

Arrow functions cannot be used to create objects or instances because they lack the `constructor`. The super keyword, on the other hand, is used in the context of `classes` and `inheritance`.

- When used in a method within a class, super refers to the parent class's prototype, allowing you to call methods from the parent class.
- When used in a class constructor, super is used to call the constructor of the parent class to initialize the object

_Arguments object is not accessible inside Arrow Function_

```javascript
// Accessing arguments object inside Regular function
function add(a, b, c) {
  console.log(arguments[0]); // 1
  console.log(arguments[1]); // 2
  console.log(arguments[2]); // 3
}
add(1, 2, 3);

// Accessing arguments object inside Arrow function
const add = (a, b, c) => {
  console.log(arguments[0]); // {}
  console.log(arguments[1]); // [Function: require]
  console.log(arguments[2]); // Object
};
add(1, 2, 3);
```

### Classes

Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are unique to classes.

Classes are in fact `special functions`, and just as you can define `function expressions` and `function declarations`, a class can be defined in two ways: a `class expression` or a `class declaration`.

```javascript
// Declaration
class Language {
  constructor(name, version) {
    this.name = name;
    this.version = version;
  }
}

// Expression: the class is anonymous but assigned to a variable
const Language = class {
  constructor(name, version) {
    this.name = name;
    this.version = version;
  }
};

// Expression: the class has its own name
const Language = class Language2 {
  constructor(name, version) {
    this.name = name;
    this.version = version;
  }
};
```

**Constructor**

The constructor method is a special method for creating and initializing an object created with a class. There can only be one special method with the name `constructor` in a class — a `SyntaxError` is thrown if the class contains more than one occurrence of a constructor method. A constructor can use the `super` keyword to call the constructor of the super class.

> Alternatively, if the instance properties' values do not depend on the constructor's arguments, you can define them as `class fields`.

```javascript
// Class Fiels don't require keywords like let or const
class Language {
  name = "Javascript";
  version;
  constructor(name, version) {
    this.name = name;
    this.version = version;
  }
}
```

**Method**

Methods are `functions` defined as part of a `class` or `object`.

```javascript
// Method
class Language {
  constructor(name, version) {
    this.name = name;
    this.version = version;
  }
  getInfo() {
    return { name: this.name, version: this.version };
  }
}
const language1 = new Language("JavaScript", "ES6");
console.log(language1.getInfo()); // {name: "JavaScript", version: "ES6"}
```

Implementing the class without using class keyword.

```javascript
function Language(name, version) {
  this.name = name;
  this.version = version;
}

Language.prototype.getInfo = function () {
  return { name: this.name, version: this.version };
};

const language1 = new Language("JavaScript", "ES6");
console.log(language1.getInfo()); // {name: "JavaScript", version: "ES6"}
```

**Static methods and fields**

The `static` keyword defines a static `method` or `field`` for a class. Static properties (fields and methods) are defined on the class itself instead of each instance.

```javascript
// Static Method and Field
class Language {
  constructor(name, version) {
    this.name = name;
    this.version = version;
  }
  static type = "Programming";
  static printType() {
    console.log(this.type);
  }
  getInfo() {
    return { name: this.name, version: this.version };
  }
}
const language1 = new Language("JavaScript", "ES6");
console.log(language1.type); // undefined
language1.printType(); // TypeError: language1.printType is not a function

// Static methods or fields are accessible directly on the class instead of class instances.
console.log(Language.type); // Programming
Language.printType(); // Programming
```

**Private**

Private fields cannot be accessed outside of the class; they can only be read or written within the class body. By defining a fied or method as private we avoid exposing any unwanted data or logic to the consumer of the class. This proved secure and also provides clean api for the consumer of the class. Private fields and methods are declared using `#` before the field or method name.

```javascript
// Private Method and Field
class Language {
  #name = "Javascript"; // used # before variable name to define private field
  version = "ES3";
  constructor(name, version) {
    this.#name = name; // used # before variable name to set value
    this.version = version;
  }
  #getInfo() {
    // prepend # to define private method
    return { name: this.name, version: this.version };
  }
}
const language1 = new Language("JavaScript", "ES6");
console.log(language1.version); // ES3
console.log(language1.#name); // SyntaxError: Private field '#name' must be declared in an enclosing class
console.log(language1.#getInfo()); // SyntaxError: Private field '#getInfo' must be declared in an enclosing class
```

**Inheritance**

A class inheriting properties of another class is called `Inheritance`. `extends` keyword to extend the properties of a another class onto itself.

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}

class Dog extends Animal {
  constructor(name) {
    super(name); // call the super class constructor and pass the name of the parameter
  }

  speak() {
    super.speak(); // using super we can access parent class methods in child class
    console.log(`${this.name} barks.`);
  }
}

const d = new Dog("Orio");
// overriden method from parent class
d.speak(); // Orio makes a noise. Orio barks.
// field accessed from parent class
console.log(d.name); // Orio
```

`Dog class` extends the properties of `Animal class`. Here Animal class is the parent class. Animal has it's own `speak` method. Dog class has overriden the existing method and defined it's own logic. Though Dog class has not field `name` we can access it on the object `d` due to inheritance. Using `super` keyword from child class, we can access fields and methods of parent class.

### Object destructuring

The destructuring assignment syntax is a JavaScript expression that makes it possible to unpack values from arrays, or properties from objects, into distinct variables.

```javascript
// Array destructuring
const x = [1, 2, 3, 4, 5];
const [y, z] = x;
console.log(y); // 1
console.log(z); // 2

// Object destructuring
const obj = { a: 1, b: 2 };
const { a, b } = obj;
console.log(a); // 1
console.log(b); // 2
```

Values from an object or array be extracted into variables using destructuring syntax.

**Default value**

Apart from extracting values into variables, we can provide default values.

```javascript
const [a = 1] = []; // a is 1
const { b = 2 } = { b: undefined }; // b is 2
const { c = 2 } = { c: null }; // c is null
const [a = "one", b = "two"] = [];
console.log(a, b); // one, two
```

The default value can be any expression. It will only be evaluated when necessary.

**Rest property**

Using `...` 3 dots before the variable name, we can store rest of the values into that variables. Destructuring an array stores an array into rest variable and similarly an object incase of object destructuring.

```javascript
const { a, ...rest } = { a: 1, b: 2, c: 3 };
console.log(rest); // { b: 2, c: 3 }

const [first, ...rest] = [1, 2, 3];
console.log(rest); // [2, 3]
```

**Assigning to new variable name**

A property can be unpacked from an object and assigned to a variable with a different name than the object property.

```javascript
const o = { p: 42, q: true };
const { p: foo, q: bar } = o;

console.log(foo); // 42
console.log(bar); // true

// with default value
const { a: aa = 10, b: bb = 5 } = { a: 3 };

console.log(aa); // 3
console.log(bb); // 5
```

Few examples for different cases of destructuring

```javascript
// Destructuring with more elements than the source
const foo = ["one", "two"];

const [red, yellow, green, blue] = foo;
console.log(red); // "one"
console.log(yellow); // "two"
console.log(green); // undefined
console.log(blue); // undefined

// Swapping variables
let a = 1;
let b = 3;

[a, b] = [b, a];
console.log(a); // 3
console.log(b); // 1

// Parsing an array returned from a function
function f() {
  return [1, 2];
}

const [a, b] = f();
console.log(a); // 1
console.log(b); // 2

// Ignoring some returned values
function f() {
  return [1, 2, 3];
}

const [a, , b] = f();
console.log(a); // 1
console.log(b); // 3

const [c] = f();
console.log(c); // 1

[, ,] = f(); // Ignoring all the values

// Destructuring only few values from rest
const [a, b, ...[c, , d]] = [1, 2, 3, 4, 5, 6]; //...[] holds [3, 4, 5, 6]
console.log(a, b, c, d); // 1 2 3 5

// Nested destructuring
const [a, b, ...[c, d, ...[e, f]]] = [1, 2, 3, 4, 5, 6];
console.log(a, b, c, d, e, f); // 1 2 3 4 5 6

// Destructuring an iterable
const [a, b] = new Map([
  [1, 2],
  [3, 4],
]);
console.log(a, b); // [1, 2] [3, 4]

// Variable object property names
const key = "z";
const { [key]: foo } = { z: "bar" };

console.log(foo); // "bar"

// Invalid JavaScript identifier as a property name
const foo = { "fizz-buzz": true };
const { "fizz-buzz": fizzBuzz } = foo;

console.log(fizzBuzz); // true
```

Few examples of destructuring function arguments

```javascript
// Destructuring function argument
function getLanguageName({ id, ...rest }) {
  return rest.name;
}
console.log(getLanguageName({ id: 1, name: "Javascript" })); // Javascript

// With new name
function getLanguageName({ name: langName }) {
  return langName;
}
console.log(getLanguageName({ id: 1, name: "Javascript" })); // Javascript

//Nested object
function getLanguageName({ name: langName, release: { date: releaseDate } }) {
  return `Name: ${langName}, Release Date: ${releaseDate}`;
}
console.log(
  getLanguageName({
    id: 1,
    name: "Javascript",
    release: { date: "mm/dd/yyyy", version: 1 },
  })
); // Name: Javascript, Release Date: mm/dd/yyyy

// With default value
function getLanguageName({ name = "Python" }) {
  return name;
}
console.log(getLanguageName({ id: 1 })); // Python
```

## Nodejs Getting Started

### What is Nodejs

![Node.js logo](/images/nodeGettingStarted/node-logo.png "Node.js logo")

Node is an open-source, `asynchronous event-driven` JavaScript `runtime environment` that allows developers to build and run JavaScript applications outside of a web browser. It is designed to be efficient, scalable, and suitable for building a wide range of networked and server-side applications. Node.js is built on the `V8 JavaScript engine` developed by Google, which is the same engine used in the Google Chrome web browser. V8 is written in C++.

JavaScript was developed to add interactivity to webpages. That is it was meant to run only on browsers. Each browser invented their own Javascript engine which runs Javascript on Browsers. `Google Chrome` has `V8`, `Mozilla` has `Spider Monkey` and `Safari` uses `Javascript Core`. Each engine has their own mechanism for performance. In the year 2009, `Ryan Dahl` came up with a solution to run Javascript out of the browser with the help of V8 Javascript engine.

Javascript doesn't come with DOM, timers and webapis. These are provided by the browser. We have a global document object in browser. This provides api to manipulate DOM nodes in browser. Browser parses the html and css and exposes apis to Javascript scope to enable DOM manipulation. DOM is not the default of Javascript. `Browser + Event Loop` powers up Javascript.

![Libuv Logo](./images/nodeGettingStarted/libuv-logo.png "Libuv Logo")

Even If we have V8 engine, we lack `Event Loop` which makes Javascript asynchronous. `Timers`, `WebApis` and `Apis` to access the system resources and Filesystem. This is where `Libuv` comes in. It provides all the other tools required to make Node.js complete.

`JavaScript` is `Single Threaded` and `Blocking`. With the help of `Event Loop` in both browser and Node, it attains the capability of being `Non Blocking`. Main code execution is handled by Javascript engine. So any code that is time consuming will block the other processes. Hence it's recommended to not used Node.js for computationally intensive tasks. Libuv enables us to make use of other threads while main thread is busy executing the code. Node.js exposes `Async methods` which runs on a seprate thread and calls the callback when the said operation is done.

### Why Nodejs

**Benefits**

1. `Non-Blocking I/O:` Node.js is known for its non-blocking, event-driven architecture, which allows it to handle a large number of concurrent connections efficiently. This makes it particularly well-suited for building real-time applications like chat applications and online gaming.

2. `JavaScript Everywhere:` With Node.js, developers can use JavaScript for both client-side and server-side development. This allows for code reuse and simplifies the development process when building full-stack applications.

3. `NPM (Node Package Manager):` Node.js comes with a built-in package manager called NPM. NPM is a vast repository of open-source libraries and modules that developers can use to extend the functionality of their Node.js applications. It simplifies dependency management and facilitates code sharing within the Node.js community.

4. `Single-Threaded Event Loop:` Node.js uses a single-threaded event loop for handling I/O operations asynchronously. While the core of Node.js is single-threaded, it leverages underlying system threads for heavy computation tasks and I/O operations, ensuring efficient resource utilization.

5. `Modules:` Node.js uses a module system that allows developers to create reusable pieces of code. CommonJS modules are the standard for organizing code in Node.js, and developers can create their own modules or use built-in ones.

6. `Active Community:` Node.js has a vibrant and active developer community, which results in regular updates, enhancements, and a wide array of libraries and frameworks available for developers to use.

Node.js is commonly used for building `web servers`, `RESTful APIs`, `real-time applications like chat applications and games`, `microservices`, and various backend services.

> It's important to note that while Node.js is excellent for certain use cases, it may not be the best choice for CPU-bound tasks. In such cases, other programming languages or runtime environments may be more suitable.

**Handling Computationally Intensive Tasks**

- A node package `pm2` enables us to run multiple instances of Node.js to handle computationaly intensive tasks. It automatically spins up new Node.js instances when in need to not block the main thread.
- Node.js ecosystem is very mature to build microservices. Load balancing and proper resource utilisation can make Node.js handle intensive tasks aswell.
- `cluster-module` is a built in Node.js module that enables spinning up new child processes to handle intensive tasks.
- `worker-threads` is a build in Node.js module that enables creating worker threads to perform intensive tasks. Worker threads removes the memory and resource overhead in comparision to `pm2` and `cluster-module`.

> As other Multi-threaded programming languages and frameworks which are suitable for computationally intensive tasks and not so suitable for handling concurrent requests are coming up with ways to make them Non-blocking, Node.js community is also ever developing to add new features to Node.js.

### Blocking and Non Blocking architectures

**Blocking**

Blocking is when the execution of additional JavaScript in the Node.js process must wait until an operation running in main thread completes. This happens because the event loop is unable to continue running JavaScript while a blocking operation is occurring. Even though libuv takes up few asynchronous tasks and runs on other threads. If the developer adds a cpu intensive task inside the callback main thread will block.

In Node.js, JavaScript that exhibits poor performance due to being CPU intensive rather than waiting on a non-JavaScript operation, such as I/O, isn't typically referred to as blocking. `Synchronous` methods in the Node.js standard library that use [`libuv`](https://libuv.org/) are the most commonly used `blocking` operations. Native modules may also have blocking methods.

All of the I/O methods in the Node.js standard library provide asynchronous versions, which are non-blocking, and accept callback functions. Some methods also have blocking counterparts, which have names that end with `Sync`. Always prefer Async methods over Sync methods.

**Blocking vs Non Blocking**

Blocking methods execute synchronously and non-blocking methods execute asynchronously.

Using the File System module as an example, this is a synchronous file read:

```javascript
const fs = require("fs");
const data = fs.readFileSync("/file.md"); // blocks here until file is read
```

And here is an equivalent asynchronous example:

```javascript
const fs = require("fs");
fs.readFile("/file.md", (err, data) => {
  if (err) throw err;
});
```

The first example appears simpler than the second but has the disadvantage of the second line blocking the execution of any additional JavaScript until the entire file is read.

> In the synchronous version if an error is thrown it will need to be caught or the process will crash. In the asynchronous version, it is up to the author to decide whether an error should throw as shown.

Let's expand the example a little bit:

```javascript
const fs = require("fs");
const data = fs.readFileSync("/file.md"); // blocks here until file is read
console.log(data);
moreWork(); // will run after console.log
```

And here is a similar, but not equivalent asynchronous example:

```javascript
const fs = require("fs");
fs.readFile("/file.md", (err, data) => {
  if (err) throw err;
  console.log(data);
});
moreWork(); // will run before console.log
```

In the first example above, `console.log` will be called before `moreWork()`. In the second example `fs.readFile()` is `non-blocking` so JavaScript execution can continue and `moreWork()` will be called first. The ability to run `moreWork()` without waiting for the file read to complete is a key design choice that allows for higher throughput.

**Concurrency and Throughput**

JavaScript execution in Node.js is single threaded, so concurrency refers to the event loop's capacity to execute JavaScript callback functions after completing other work. Any code that is expected to run in a concurrent manner must allow the event loop to continue running as non-JavaScript operations, like I/O, are occurring.

As an example, let's consider a case where each request to a web server takes 50ms to complete and 45ms of that 50ms is database I/O that can be done asynchronously. Choosing non-blocking asynchronous operations frees up that 45ms per request to handle other requests. This is a significant difference in capacity just by choosing to use non-blocking methods instead of blocking methods.

The event loop is different than models in many other languages where additional threads may be created to handle concurrent work.

**Dangers of Mixing Blocking and Non-Blocking Code**

There are some patterns that should be avoided when dealing with I/O. Let's look at an example:

```javascript
const fs = require("fs");
fs.readFile("/file.md", (err, data) => {
  if (err) throw err;
  console.log(data);
});
fs.unlinkSync("/file.md");
```

In the above example, `fs.unlinkSync()` is likely to be run before `fs.readFile()`, which would delete `file.md` before it is actually read. A better way to write this, which is completely non-blocking and guaranteed to execute in the correct order is:

```javascript
const fs = require("fs");
fs.readFile("/file.md", (readFileErr, data) => {
  if (readFileErr) throw readFileErr;
  console.log(data);
  fs.unlink("/file.md", (unlinkErr) => {
    if (unlinkErr) throw unlinkErr;
  });
});
```

The above places a `non-blocking` call to `fs.unlink()` within the callback of `fs.readFile()` which guarantees the correct order of operations.

## Node Internal Architecture

### V8 Engine

V8 is the name of the JavaScript engine that powers Google Chrome. It's the thing that takes our JavaScript and executes it while browsing with Chrome. V8 provides the runtime environment in which JavaScript executes. The DOM and the other Web Platform APIs are provided by the browser. V8 is written in C++, and it's continuously improved. It is portable and runs on Mac, Windows, Linux and several other systems.

The cool thing is that the JavaScript engine is independent of the browser in which it's hosted. This key feature enabled the rise of Node.js. V8 was chosen to be the engine that powered Node.js back in 2009, and as the popularity of Node.js exploded, V8 became the engine that now powers an incredible amount of server-side code written in JavaScript.

**Other Javascript engines**

- `Firefox` has `SpiderMonkey`
- `Safari` has `JavaScriptCore (also called Nitro)`
- `Edge` was originally based on `Chakra` but has more recently been rebuilt using `Chromium` and the `V8` engine.

All those engines implement the ECMA ES-262 standard, also called ECMAScript, the standard used by JavaScript.

**What V8 does**

V8 is a single threaded execution engine. It’s built to run exactly one thread per JavaScript execution context. You can actually run two V8 engines in the same process — e.g. web-workers, but they won’t share any variables or context like real threads. This doesn’t mean V8 is running on a single thread, but it does mean it provides a JavaScript flow of a single thread.

On the runtime, V8 is mainly managing the heap memory allocation and the single threaded call stack. The call stack is mainly a list of function to execute, by calling order. Every function which calls another function will be inserted one after the other directly, and callbacks will be sent to the end. This is actually why calling a function with setTimeout of zero milliseconds sends it to the end of the current line and doesn’t call it straight away (0 milliseconds).

**JS Interpreter — Ignition & Optimization Compiler — TurboFan & Crankshaft**

V8 gets its speed from just-in-time (JIT) compilation of JavaScript to native machine code, just before executing it. First of all, the code is compiled by a baseline compiler, which quickly generates non-optimized machine code. On runtime, the compiled code is analyzed and can be re-compiled for optimal performance. Ignition provides the first while TruboFan & Crankshaft the second.

JIT compilation result machine code can take a large amount of memory, while it might be executed once. This is solved by the Ignition, which is executing code with less memory overhead.

The TurboFan project started in 2013 to improve the weakness of Crankshaft which isn't optimized for some part of the JavaScript functionality e.g. error handling. It was designed for optimizing both existing and future planned features at the time.

![V8 Architecture](./images/v8-architecture.webp "V8 Architecture")

**WebAssembly — Liftoff**

Achieving great performance is also key in the browser, and this is the task Liftoff is used for — generating machine code. Not using the complex multi-tier compilation, Liftoff is a simpler code generator, which generates code for each opcode (a single portion of machine code, specifying an operation to be performed) at a time. Liftoff generates code much faster than TurboFan (~10x) which is obviously less performant (~50%).

**Garbage Collection — Orinoco**

Running over the memory heap, looking for disconnected memory allocations is the Orinoco. Implementing a generational garbage collector, moving objects within the young generation, from the young to the old generation, and within the old generation. These moves leave holes, and Orinoco performs both evacuation and compaction to free space for more objects.

Another optimization performed by Orinoco is in the way it searches through the heap to find all pointers that contain the old location of the objects moved and update them with the new location. This is made using a data structure called remembered set.

On top of these, black allocation is added, which basically means the garbage collection process automatically marks living objects in black in order to speed up the iterative marking process.

### Libuv

libuv is a multi-platform support library written in C with a focus on asynchronous I/O. It was primarily developed for use by `Node.js`. It’s designed around the event-driven asynchronous I/O model.

libuv is responsible for Node's anynchronous behavour. Whenever Node's main thread encounters an asynchronous function, it transfers the work to libuv. Libuv executes that asynchronous function and calls the callback passed to async function on completion. While libuv is busy performing intensive task, Node's main thred continues code execution without stopping.

Lets see an example of Asynchronous Node in action which uses libuv under the hood.

```javascript
// Blocking code
const crypto = require("node:crypto");
const iterations = 1;

console.time("executionTime");

for (let i = 0; i < iterations; i++) {
  crypto.pbkdf2Sync("password", "salt", 100000, 512, "sha512"); // Any method with Sync keyword is blocking
}
console.timeEnd("executionTime");
```

On incrementing the iteration cout, we can see the execution time. Below are the time taken in my hardware. It might vary for you.

```bash +@output
executionTime: 961.725ms // iteration 1
executionTime: 1.843s // iteration 2
executionTime: 3.060s // iteration 3
```

As you can see from the execution time took for each iteration is increasing linearly. That is, 1 task takes 1(T) of time, 2 takes 2(T). N task takes N(T) time.

| Iteration | Time(ms) |
| :-------- | :------- |
| 1         | 961.725  |
| 2         | 1843     |
| 3         | 3060     |

```javascript
// Non Blocking code
const crypto = require("node:crypto");
const iterations = 3;

const start = Date.now();
for (let i = 0; i < iterations; i++) {
  crypto.pbkdf2("password", "salt", 100000, 512, "sha512", () => {
    // No sync keyword says its asynchronous
    console.log("Hashed");
    console.log("executionTime:", Date.now() - start);
  });
}
```

```bash +@output
executionTime: 911 // iteration 1
executionTime: 1155 // iteration 2
executionTime: 1536 // iteration 3
```

`pbkdf2` is not a synchronous function. Main thread hands over the execution to libuv so even with 3 iterations time taken is `1536 milliseconds`. Processes are run parallely. With synchronous approach it took `3060 milliseconds` to perform 3 iterations. With Asynchronous approach that time reduced to `1536 milliseconds`.

| Iteration | Time(ms) |
| :-------- | :------- |
| 1         | 911      |
| 2         | 1155     |
| 3         | 1536     |

The library provides much more than a simple abstraction over different I/O polling mechanisms: ‘handles’ and ‘streams’ provide a high level abstraction for sockets and other entities; cross-platform file I/O and threading functionality is also provided, amongst other things.

Here is a diagram illustrating the different parts that compose libuv and what subsystem they relate to:

![LibUV Architecture](./images//libuv-architecture.webp "LibUV Architecture")

**Handles and requests**

libuv provides users with 2 abstractions to work with, in combination with the event loop: handles and requests.

Handles represent long-lived objects capable of performing certain operations while active. Some examples:

A prepare handle gets its callback called once every loop iteration when active.

A TCP server handle that gets its connection callback called every time there is a new connection.

Requests represent (typically) short-lived operations. These operations can be performed over a handle: write requests are used to write data on a handle; or standalone: getaddrinfo requests don’t need a handle they run directly on the loop.

**The I/O loop**

The I/O (or event) loop is the central part of libuv. It establishes the content for all I/O operations, and it’s meant to be tied to a single thread. One can run multiple event loops as long as each runs in a different thread. The libuv event loop (or any other API involving the loop or handles, for that matter) is not thread-safe except where stated otherwise.

The event loop follows the rather usual single threaded asynchronous I/O approach: all (network) I/O is performed on non-blocking sockets which are polled using the best mechanism available on the given platform: epoll on Linux, kqueue on OSX and other BSDs, event ports on SunOS and IOCP on Windows. As part of a loop iteration the loop will block waiting for I/O activity on sockets which have been added to the poller and callbacks will be fired indicating socket conditions (readable, writable hangup) so handles can read, write or perform the desired I/O operation.

In order to better understand how the event loop operates, the following diagram illustrates all stages of a loop iteration:

![Libuv Loop Iteration](./images/libuv_loop_iteration.webp "Libuv Loop Iteration")

1. The loop concept of ‘now’ is initially set.

2. Due timers are run if the loop was run with UV_RUN_DEFAULT. All active timers scheduled for a time before the loop’s concept of now get their callbacks called.

3. If the loop is alive an iteration is started, otherwise the loop will exit immediately. So, when is a loop considered to be alive? If a loop has active and ref’d handles, active requests or closing handles it’s considered to be alive.

4. Pending callbacks are called. All I/O callbacks are called right after polling for I/O, for the most part. There are cases, however, in which calling such a callback is deferred for the next loop iteration. If the previous iteration deferred any I/O callback it will be run at this point.

5. Idle handle callbacks are called. Despite the unfortunate name, idle handles are run on every loop iteration, if they are active.

6. Prepare handle callbacks are called. Prepare handles get their callbacks called right before the loop will block for I/O.

7. Poll timeout is calculated. Before blocking for I/O the loop calculates for how long it should block. These are the rules when calculating the timeout:

8. The loop blocks for I/O. At this point the loop will block for I/O for the duration calculated in the previous step. All I/O related handles that were monitoring a given file descriptor for a read or write operation get their callbacks called at this point.

9. Check handle callbacks are called. Check handles get their callbacks called right after the loop has blocked for I/O. Check handles are essentially the counterpart of prepare handles.

10. Close callbacks are called. If a handle was closed by calling uv_close() it will get the close callback called.

11. The loop concept of ‘now’ is updated.

12. Due timers are run. Note that ‘now’ is not updated again until the next loop iteration. So if a timer became due while other timers were being processed, it won’t be run until the following event loop iteration.

13. Iteration ends. If the loop was run with UV_RUN_NOWAIT or UV_RUN_ONCE modes the iteration ends and uv_run() will return. If the loop was run with UV_RUN_DEFAULT it will continue from the start if it’s still alive, otherwise it will also end.

> libuv uses a thread pool to make asynchronous file I/O operations possible, but network I/O is always performed in a single thread, each loop’s thread.

**File I/O**

Unlike network I/O, there are no platform-specific file I/O primitives libuv could rely on, so the current approach is to run blocking file I/O operations in a thread pool.

**Networking**

Node.js is often used for building networked applications, such as web servers and chat servers. libuv provides networking capabilities that allow Node.js to create and manage network sockets, handle incoming connections, and perform network operations asynchronously.

**Timers and Callbacks**

libuv includes a timer and callback management system. It allows Node.js to schedule functions to be executed at specific times or after specific intervals. This is essential for implementing timeouts, intervals, and other time-dependent operations in Node.js applications.

### Event Loop Architecture

Event Loop is part of libuv. Using thread pool it runs tasks delegated as asynchronous. Once the asyncronous action is complete, libuv pushes its corresponding callback to event loop queue. There are multiple Queues. Based on Priority these callback queues are pushed back to `CallStack` for execution.

![Asynchronous Node.js](./images/node-architecture/libuv-eventloop-architecture.png "Asynchronous Node.js")

```javascript
console.log("First");
setTimeout(() => {
  console.log("Run in Timeout");
}, 0);
console.log("Last");
```

```bash +@output
First
Last
Run in Timeout
```

Even though we passed 0 milliseconds to setTimeout function, it runs after `Last` is logged to the console. This is because setTimeout is an Async function. Callback inside it takes a longer route in the queue to get processed. Keeping track of the timer is handled by the thread pool.

**Thread Pool**

Threads are the numbers of cpu's or cores present on the computer. Node.js runs on a single thread/core. Rest of the cores are at Libuv's disposal. Async functions are run on these thread pool(cores/cpu's) by libuv. On completion, callbacks are pushed to Event Loop.

```javascript
const crypto = require("node:crypto");

const ITERATIONS = 5;

const start = Date.now();

for (let i = 0; i < ITERATIONS; i++) {
  crypto.pbkdf2("password", "salt", 10000, 512, "sha512", () => {
    console.log(`Hash: ${i + 1} `, Date.now() - start);
  });
}
```

```bash +@output
Hash: 2  199
Hash: 4  200
Hash: 1  200
Hash: 3  203
Hash: 5  302
```

In the above example we called crypto modules async function to create an hash. From the output we see time it took for each iteration. The average of first 4 iterations comes around 200. But the 5th iteration took 50% extra time. This is bec,ause of `thread pool size`. There is a default thread pool size of `4`. Lets see how we can modify that.

`process.env.UV_THREADPOOL_SIZE = 8;` updates the default thread pool size. Now after setting pool size to 8 and setting the iterations count to 6 lets see the output timings.

```bash +@output
Hash: 3  183
Hash: 4  190
Hash: 1  191
Hash: 2  191
Hash: 5  309
Hash: 6  312
```

Even after increasing the thread pool size, 5th and 6th iterations are 50% more time. Why is that?. Its because of system resource restriction. Number of CPU's/cores on my computer is 4. I cannot increase the thread pool size beyond hardware capabilities. Make sure to update thread pool size within hardware bounds.

**Native Async Mechanism**

```javascript
const https = require("node:https");
const ITERATIONS = 4;
const start = Date.now();
for (let i = 0; i < ITERATIONS; i++) {
  https
    .request("https://google.com", (res) => {
      res.on("data", () => {});
      res.on("end", () => {
        console.log(`Request: ${i + 1} `, Date.now() - start);
      });
    })
    .end();
}
```

```bash +@output
Request: 2  499
Request: 1  530
Request: 3  535
Request: 4  541
```

We are making api call to `google.com`. Average response time is 500 milliseconds. This may vary based on internet speed. Lets increase the number of iterations and see the behaviour.

```bash +@output
Request: 1  479
Request: 4  498
Request: 2  502
Request: 5  509
Request: 6  515
Request: 3  530
Request: 7  540
Request: 8  547
```

Even with 8 iterations, average response time remains same. With 4 cores in my computer, this time should have gone up similar to hashing. That is not the case. Operating system provides Native Async methods to handle network calls. Kernel handles the network calls. There are different mechanisms in different OS. In `Linux` its called `epoll`, `KQueue` in `Mac OS`, `IO Port` in `Windows`. For Network I/O tasks thread pool is not used instead kernel handles it. Other operations like reading file system don't have native methods, hence thread pool is used there.

> Network I/O operations doesn't depend on thread pool. Kernel handles them and libuv polls the kernel to check the completion. If completed libuv pushes the callback into Event Loop.

### Event Loop Queues

Node.js Event Loop is different from Browser Event Loop. Node.js manages callback queues differently. Lets see how. Event Loop consists of `MicroTask Queue`(includes `nextTick Queue` and `Promise Queue`), `Timer Queue`, `I/O Queue`, `Check Queue`, `Close Queue`.

> All Synchronous actions take priority over all async actions. Even if we multiple callbacks waiting in Event Loop, Synchronous action gets pushed to callstack first. This creates `starvation`. Hence it's recommended to not run anything cpu intensive in the main thread. It blocks the rest of the functionality.

Lets see how these queues are handled individually

**MicroTask Queue**

MicroTask Queue consists of 2 queues. `NextTick Queue` and `Promise Queue`. To push a callback to NextTick Queue we use `process.nextTick()` and to push to Promise queue we resolve or reject a promise.

```javascript
// All Synchronous actions take priority over Async actions
console.log("First");
process.nextTick(() => console.log("Inside next tick"));
console.log("Last");
```

Output:

```bash +@output
First
Last
Inside next tick
```

Lets compare `NextTick Queue` with `Promise Queue`.

```javascript
console.log("First");
Promise.resolve().then(() => console.log("Inside promise"));
process.nextTick(() => console.log("Inside NextTick"));
console.log("Last");
```

Output:

```bash +@output
First
Last
Inside NextTick
Inside promise
```

We see that NextTick takes priority over Promise Queue.

**Timer Queue**

Time is populated with callbacks returned from `setTimeout` `setInterval`. `MicroTask Queue` takes priority over `Time Queue`.

```javascript
setTimeout(() => console.log("setTimeout"), 0);
Promise.resolve().then(() => console.log("Inside promise"));
process.nextTick(() => console.log("Inside NextTick"));
```

Output:

```bash +@output
Inside NextTick
Inside promise
setTimeout
```

setTimeout gets logged in the end even though it comes first.

```javascript
setTimeout(() => console.log("setTimeout 1"), 0);
setTimeout(() => {
  console.log("setTimeout 2");
  process.nextTick(() => console.log("NextTick inside setTimeout"));
}, 0);

Promise.resolve().then(() => console.log("promise 1"));
process.nextTick(() => console.log("NextTick 1"));
setTimeout(() => console.log("setTimeout 3"), 0);
```

Output:

```bash +@output
NextTick 1
promise 1
setTimeout 1
setTimeout 2
NextTick inside setTimeout
setTimeout 3
```

From the 2nd example we see that, `NextTick inside setTimeout` is logged first and then `setTimeout 3` is logged. This is because `MicroTask Queue` is checked and executed in between each callback of `Timer Queue`.

**I/O Queue**

I/O Queue is populated with callbacks of I/O operations. Example file read or Network calls.

```javascript
const fs = require("node:fs");

setTimeout(() => console.log("setTimeout 1"), 0);
fs.readFile("file.txt", (data) => {
  console.log("read file");
});
Promise.resolve().then(() => console.log("promise 1"));
process.nextTick(() => console.log("NextTick 1"));
setTimeout(() => console.log("setTimeout 2"), 0);
```

Output:

```bash +@output
NextTick 1
promise 1
setTimeout 1
setTimeout 2
read file
```

Priority order goes like this: microTasks Queue > Timer Queue > I/O Queue.

Lets see a scenario with Timer queue and I/O queue

```javascript
const fs = require("node:fs");
setTimeout(() => console.log("setTimeout 1"), 0);
fs.readFile("file.txt", (data) => {
  console.log("read file");
});
```

Output:

```bash +@output
setTimeout 1
read file
============
setTimeout 1
read file
============
read file
setTimeout 1
```

If we run the above code multiple times, same output is not guaranteed. This is because of how `setTimeout` handles 0 milliseconds. If 0 is passed, default value will be taken as 1. Any value greater than 0 will be taken as is. Due to this behaviour of setTimeout, outputs may vary on multiple runs with Timer Queue and I/O Queue.

**Check Queue**

Callbacks are pushed to Check Queue using `setImmediate()` this is specific to Node.js. This is not accessible to browser Javascript.

```javascript
const fs = require("node:fs");
fs.readFile(__filename, (data) => {
  console.log("read file 1");
});
Promise.resolve().then(() => console.log("promise 1"));
process.nextTick(() => console.log("NextTick 1"));
setTimeout(() => console.log("setTimeout 1"), 0);
setImmediate(() => console.log("setImmediate 1"));
for (let i = 0; i < 1000000000; i++) {}
```

Output:

```bash +@output
NextTick 1
promise 1
setTimeout 1
setImmediate 1
read file 1
```

According to the the Event Loop lifecycle, `I/O Queue` callbacks should be processed before `Check Queue`. But in the output we see `setImmediate 1` logged before `read file 1`.

This behaviour is because of `I/O Polling`. First `MicroTask Queue` is processed. Then `Timer Queue`. When the control comes to `I/O Queue`, callback from read file should be present in the queue. But it wont be populated untill polling is complete. Polling is done after checking I/O Queue.

> `Polling` is where libuv talks to kernel or thread pool to check for I/O task completion. Only completed action's callbacks are populated into I/O Queue.

Once polling is done control goes to `Check Queue`. In the next iteration of the event loop callbacks in the `I/O Queue` is handled.

MicroTask Queue is processed before Check Queue.

```javascript
const fs = require("node:fs");
fs.readFile(__filename, (data) => {
  console.log("read file 1");
  Promise.resolve().then(() => console.log("inside promise "));
  process.nextTick(() => console.log("inside NextTick "));
  setImmediate(() => console.log("inside setImmediate "));
});
Promise.resolve().then(() => console.log("promise 1"));
process.nextTick(() => console.log("NextTick 1"));
setTimeout(() => console.log("setTimeout 1"), 0);
setImmediate(() => console.log("setImmediate 1"));
for (let i = 0; i < 1000000000; i++) {}
```

Output:

```bash +@output
NextTick 1
promise 1
setTimeout 1
setImmediate 1
read file 1
inside NextTick
inside promise
inside setImmediate
```

In the above output we can see that `inside NextTick` and `inside promise` are logged before `inside setImmediate`. After polling MicroTask Queue is processed before Check Queue.

**Close Queue**

Calling a function on `close` event pushes that function to `Close Queue`.

```javascript
const fs = require("node:fs");

const readableStream = fs.createReadStream(__filename);
readableStream.close();
readableStream.on("close", () => console.log("closing readable stream"));
Promise.resolve().then(() => console.log("promise 1"));
process.nextTick(() => console.log("NextTick 1"));
setTimeout(() => console.log("setTimeout 1"), 0);
setImmediate(() => console.log("setImmediate 1"));

for (let i = 0; i < 1000000000; i++) {}
```

Output:

```bash +@output
NextTick 1
promise 1
setTimeout 1
setImmediate 1
closing readable stream
```

From the above example, we see the order of execution. Close Queue is processed at the end.

**Points to remember**

1. `process.nextTick()` is used to push callbacks into `NextTick Queue`.
2. A `Promise` is resolved or rejected to push callbacks into `Promise Queue`.
3. `setTimeout/setInterval` is used to push callbacks into `Timer Queue`.
4. All the `I/O` operation callbacks are pushed in `I/O Queue`.
5. `Polling` is where libuv checks with kernel and thread pool for the status of I/O tasks. If tasks are complete respective callbacks are pushed into `I/O Queue`.
6. `setImmediate` is used to push callbacks into `Check Queue`.
7. `close` event callbacks are pushed into `Close Queue`.
8. `MicroTask Queue` is processed between each type of queue and inbetween each callback of `Timer Queue` and `Check Queue`.

### Event driven Architecture

Most of Node’s objects — like HTTP requests, responses, and streams — implement the EventEmitter module so they can provide a way to emit and listen to events.

The simplest form of the event-driven nature is the callback style of some of the popular Node.js functions — for example, fs.readFile. In this analogy, the event will be fired once (when Node is ready to call the callback) and the callback acts as the event handler.

The original way Node handled asynchronous events was with callback. This was a long time ago, before JavaScript had native promises support and the async/await feature.

Callbacks are basically just functions that you pass to other functions. This is possible in JavaScript because functions are first class citizens.

It’s important to understand that callbacks do not indicate an asynchronous call in the code. A function can call the callback both synchronously and asynchronously.

In modern JavaScript, we have promise objects. Promises can be an alternative to callbacks for asynchronous APIs. Instead of passing a callback as an argument and handling the error in the same place, a promise object allows us to handle success and error cases separately and it also allows us to chain multiple asynchronous calls instead of nesting them.

```javascript
// With Then and Catch
readFileAsArray("./info.txt")
  .then((data) => {
    console.log("data:", data);
  })
  .catch(console.error);
```

Instead of passing in a callback function, we called a .then function on the return value of the host function. This .then function usually gives us access to the same lines array that we get in the callback version, and we can do our processing on it as before. To handle errors, we add a .catch call on the result and that gives us access to an error when it happens.

Making the host function support a promise interface is easier in modern JavaScript thanks to the new Promise object. Here’s the readFileAsArray function modified to support a promise interface in addition to the callback interface it already supports:

```javascript
// With Promise
const readFileData = function (file, cb = () => {}) {
  return new Promise((resolve, reject) => {
    fs.readFile(file, function (err, data) {
      if (err) {
        reject(err);
        return cb(err);
      }
      resolve(data);
      cb(null, lines);
    });
  });
};
```

So we make the function return a Promise object, which wraps the fs.readFile async call. The promise object exposes two arguments, a resolve function and a reject function.

Whenever we want to invoke the callback with an error we use the promise reject function as well, and whenever we want to invoke the callback with data we use the promise resolve function as well.

The only other thing we needed to do in this case is to have a default value for this callback argument in case the code is being used with the promise interface. We can use a simple, default empty function in the argument for that case: () => {}.

**Consuming promises with async/await**

Adding a promise interface makes your code a lot easier to work with when there is a need to loop over an async function. With callbacks, things become messy.

Promises improve that a little bit, and function generators improve on that a little bit more. This said, a more recent alternative to working with async code is to use the async function, which allows us to treat async code as if it was synchronous, making it a lot more readable overall.

Here’s how we can consume the readFileAsArray function with async/await:

```javascript
async function countOdd() {
  try {
    const lines = await readFileAsArray("./numbers");
    const numbers = lines.map(Number);
    const oddCount = numbers.filter((n) => n % 2 === 1).length;
    console.log("Odd numbers count:", oddCount);
  } catch (err) {
    console.error(err);
  }
}
countOdd();
```

We first create an async function, which is just a normal function with the word async before it. Inside the async function, we call the readFileAsArray function as if it returns the lines variable, and to make that work, we use the keyword await. After that, we continue the code as if the readFileAsArray call was synchronous.

To get things to run, we execute the async function. This is very simple and more readable. To work with errors, we need to wrap the async call in a try/catch statement.

With this async/await feature, we did not have to use any special API (like .then and .catch). We just labeled functions differently and used pure JavaScript for the code.

We can use the async/await feature with any function that supports a promise interface. However, we can’t use it with callback-style async functions.

**The EventEmitter Module**

The EventEmitter is a module that facilitates communication between objects in Node. EventEmitter is at the core of Node asynchronous event-driven architecture. Many of Node’s built-in modules inherit from EventEmitter.

The concept is simple: emitter objects emit named events that cause previously registered listeners to be called. So, an emitter object basically has two main features:

Emitting name events.
Registering and unregistering listener functions.
To work with the EventEmitter, we just create a class that extends EventEmitter.

```javascript
//  class that extends EventEmitter.
class MyEmitter extends EventEmitter {}

// Emitter instance
const myEmitter = new MyEmitter();

// Listener
myEmitter.on("customEvent", () => console.log("Got event!"));

// Emitting a named event
myEmitter.emit("something-happened");
```

Emitting an event is the signal that some condition has occurred. This condition is usually about a state change in the emitting object.

We can add listener functions using the on method, and those listener functions will be executed every time the emitter object emits their associated name event.

**Asynchronous Events**

```javascript
const fs = require("fs");
const EventEmitter = require("events");

class WithTime extends EventEmitter {
  execute(asyncFunc, ...args) {
    this.emit("begin");
    console.time("execute");
    asyncFunc(...args, (err, data) => {
      if (err) {
        return this.emit("error", err);
      }

      this.emit("data", data);
      console.timeEnd("execute");
      this.emit("end");
    });
  }
}

const withTime = new WithTime();

withTime.on("begin", () => console.log("About to execute"));
withTime.on("end", () => console.log("Done with execute"));

withTime.execute(fs.readFile, __filename);
```

The WithTime class executes an asyncFunc and reports the time that’s taken by that asyncFunc using console.time and console.timeEnd calls. It emits the right sequence of events before and after the execution. And also emits error/data events to work with the usual signals of asynchronous calls.

We test a withTime emitter by passing it an fs.readFile call, which is an asynchronous function. Instead of handling file data with a callback, we can now listen to the data event.

When we execute this code , we get the right sequence of events, as expected, and we get a reported time for the execution, which is helpful:

```javascript +@output
About to execute
execute: 4.507ms
Done with execute
```

Note how we needed to combine a callback with an event emitter to accomplish that. If the asynFunc supported promises as well, we could use the async/await feature to do the same:

```javascript
class WithTime extends EventEmitter {
  async execute(asyncFunc, ...args) {
    this.emit("begin");
    try {
      console.time("execute");
      const data = await asyncFunc(...args);
      this.emit("data", data);
      console.timeEnd("execute");
      this.emit("end");
    } catch (err) {
      this.emit("error", err);
    }
  }
}
```

**Events Arguments and Errors**

The error event is usually a special one. In our callback-based example, if we don’t handle the error event with a listener, the node process will actually exit.

To demonstrate that, make another call to the execute method with a bad argument:

```javascript
class WithTime extends EventEmitter {
  execute(asyncFunc, ...args) {
    console.time("execute");
    asyncFunc(...args, (err, data) => {
      if (err) {
        return this.emit("error", err); // Not Handled
      }

      console.timeEnd("execute");
    });
  }
}

const withTime = new WithTime();

withTime.execute(fs.readFile, ""); // BAD CALL
withTime.execute(fs.readFile, __filename);
```

The first execute call above will trigger an error. The node process is going to crash and exit:

```javascript +@output
events.js:163
      throw er; // Unhandled 'error' event
      ^
Error: ENOENT: no such file or directory, open '
```

The second execute call will be affected by this crash and will potentially not get executed at all.

If we register a listener for the special error event, the behavior of the node process will change. For example:

```javascript +@output
withTime.on("error", (err) => {
  // do something with err, for example log it somewhere
  console.log(err);
});
```

If we do the above, the error from the first execute call will be reported but the node process will not crash and exit. The other execute call will finish normally:

```javascript +@output
{ Error: ENOENT: no such file or directory, open '' errno: -2, code: 'ENOENT', syscall: 'open', path: '' }
execute: 4.276ms
```

Note that Node currently behaves differently with promise-based functions and just outputs a warning, but that will eventually change:

```javascript +@output
UnhandledPromiseRejectionWarning: Unhandled promise rejection (rejection id: 1): Error: ENOENT: no such file or directory, open ''
DeprecationWarning: Unhandled promise rejections are deprecated. In the future, promise rejections that are not handled will terminate the Node.js process with a non-zero exit code.
```

The other way to handle exceptions from emitted errors is to register a listener for the global uncaughtException process event. However, catching errors globally with that event is a bad idea.

The standard advice about uncaughtException is to avoid using it, but if you must do (say to report what happened or do cleanups), you should just let the process exit anyway:

```javascript
process.on("uncaughtException", (err) => {
  // something went unhandled.
  // Do any cleanup and exit anyway!

  console.error(err); // don't do just that.

  // FORCE exit the process too.
  process.exit(1);
});
```

However, imagine that multiple error events happen at the exact same time. This means the uncaughtException listener above will be triggered multiple times, which might be a problem for some cleanup code. An example of this is when multiple calls are made to a database shutdown action.

The EventEmitter module exposes a once method. This method signals to invoke the listener just once, not every time it happens. So, this is a practical use case to use with the uncaughtException because with the first uncaught exception we’ll start doing the cleanup and we know that we’re going to exit the process anyway.

**Order of Listeners**

If we register multiple listeners for the same event, the invocation of those listeners will be in order. The first listener that we register is the first listener that gets invoked.

```javascript
// First
withTime.on("data", (data) => {
  console.log(`Length: ${data.length}`);
});

// Second
withTime.on("data", (data) => {
  console.log(`Characters: ${data.toString().length}`);
});

withTime.execute(fs.readFile, __filename);
```

The above code will cause the “Length” line to be logged before the “Characters” line, because that’s the order in which we defined those listeners.

If you need to define a new listener, but have that listener invoked first, you can use the prependListener method:

```javascript
// First
withTime.on("data", (data) => {
  console.log(`Length: ${data.length}`);
});

// Second
withTime.prependListener("data", (data) => {
  console.log(`Characters: ${data.toString().length}`);
});

withTime.execute(fs.readFile, __filename);
```

The above will cause the “Characters” line to be logged first.

And finally, if you need to remove a listener, you can use the removeListener method.

### Multithreading in Node.js

`Javascript` is `Single threaded` and `Blocking`. `Node.js` is `Asynchronous` and `Non Blocking` Javascript `runtime`. This is possible with the help of `libuv`. Even with Non Blocking architecture Node.js runs on single thread(core/cpu). When a computationaly intensive task is loaded into main thread, `Event Loop` starves. Rest of the functionality is blocked until main thread becomes free. Node.js cannot make use of other cores available and having performant multi core processor is useless.

This is why it's recommended not to use Node.js for Computationally intensive tasks. But Node.js allows us to make the full use of rest of the cores available in the system.

```javascript
const http = require("node:http");
const server = http.createServer((req, res) => {
  if (req.url === "/first") {
    res.end("First");
  } else if (req.url === "/second") {
    for (let i = 0; i < 4000000000; i++) {}
    res.end("Second");
  }
});

server.listen(8080, () => console.log("server listening on PORT:", 8080));
```

Make the api call from browser to `localhost:8080/first`. Open the `network` tab to see the response time. Do the same for `/first` and `/second`. It took 4 seconds to get the response for second route and 5 milliseconds to get the response for first route. You might have a different response time. This is because we have a computationally intensive task in second route.

Now lets make the calls parallely. First call second route and then call the first route while second route is still loading. Now we see time taken for first route is also increased by several folds.

Second route has cpu intensive operation which takes over the main thread and delays other responses.

Lets see different ways to use other cores of the system in Node.js

**Cluster Module**

```javascript
const cluster = require("node:cluster");
const http = require("node:http");
if (cluster.isMaster) {
  console.log(`Master process ${process.pid} running`);
  cluster.fork();
  cluster.fork();
} else {
  console.log(`Worker process ${process.pid} running`);
  const server = http.createServer((req, res) => {
    if (req.url === "/first") {
      res.end("First");
    } else if (req.url === "/second") {
      for (let i = 0; i < 4000000000; i++) {}
      res.end("Second");
    }
  });
  server.listen(8080, () => console.log("server listening on PORT:", 8080));
}
```

```bash +@output
Master process 244 running
Worker process 15224 running
server listening on PORT: 8080
Worker process 2240 running
server listening on PORT: 8080
```

Master the code executing in the main js file. 2 worker processes have been spawned with `cluster.fork()` command.

Now on Parallely requesting, second route isn't blocking the first request. `Cluster` module creates a new instance of Node.js with its own Event Loop and V8 engine.

> Note: Make sure not to fork more worker threads than hardware can afford. It'll just increase increase the response time of each request.

> `pm2` an npm package manages all this for us.

**Worker Threads Module**

```js +index.js
const http = require("node:http");
const { Worker } = require("node:worker_threads");

const server = http.createServer((req, res) => {
  if (req.url === "/first") {
    res.end("First");
  } else if (req.url === "/second") {
    const iterations = 4000000000;
    const worker = new Worker("./workerThread.js", {
      workerData: { iterations },
    });
    worker.on("error", (err) => {
      console.log("Error:", err);
      res.end(err);
    });
    worker.on("message", (data) => {
      console.log("data", data);
      res.end(`Second ${data}`);
    });
  }
});

server.listen(8080, () => console.log("server listening on PORT:", 8080));
```

```js -workerThread.js
const { workerData, parentPort } = require("node:worker_threads");
console.log("iterations:", workerData.iterations);
let j = 0;
for (let i = 0; i < workerData.iterations; i++) {
  j++;
}
parentPort.postMessage(j);
```

This behaves same as `cluster` module. Make parallel request from browser and see the response times.

worker threads run in their own context. They dont share memory. worker threads allow us to pass and receive data. Using workerData object we can send data. Using parentPort we can receive message from worker thread file.

`worker_threads` module makes use of threads to compute the result. Instead of creating an entire Node.js instance which creates memory overhead.

Make use of `worker_threads` in most of the cases where you need to perform some time consuming task. Only rely on `cluster` module if you need an entire Node.js instance.

## Node Programming Getting Started

### How to Javascript on Node.js

As we all know Node.js enables us to run Javascript outside of browser environment. Node.js allows us to run Javascript in few ways.

**REPL Mode**

`REPL stands for Read Eval Print Loop`. We have something similar in browser console. Browser exposes REPL in Developer console. It allows us to run Javascript and see the output of an expression.

Run `node` from your terminal. It opens a REPL instance where we can insert Javascript expressions.

```bash +@output
Welcome to Node.js v18.17.1.
Type ".help" for more information.
>
```

It prints out the Node.js version and arrow at the end waiting for an expression. Lets run some javascript and see.

```bash +@output
> 1+2 // adding 2 numbers
3
> const str1 = "Hello" //defining a variable
undefined
> const str2 = "World" // defining a variable
undefined
> str1 +" "+ str2 // string concatination
'Hello World'
> [1, 2, 3].forEach(num=>console.log(num)) // looping over an array of numbers
1
2
3
undefined
>
```

Press `Ctrl + c` twice to exit out of the REPL.

REPL has memory, it remembers any declarations and resolves any Javascript expression. This is fine for quickly checking how Javascript behaves. We cannot write a server like this. We need a file system. Lets see how to run Javascript from a file.

**Running .js file**

We can write all out Javascript inside a .js file and run it using Node.js

```javascript
console.log("Hello World");
```

Output:

```bash +@output
node .\index.js // Running the index.js file
Hello World  // Output
```

### Isomorphic Javascript

The term "Isomorphic JavaScript" may sound complex, but at its core, it represents a powerful concept in web development that aims to bridge the gap between server-side and client-side rendering. Isomorphic JavaScript, also known as Universal JavaScript, enables developers to write code that can run seamlessly on both the server and the client, offering numerous benefits for web applications. In this blog, we'll explore what Isomorphic JavaScript is, why it matters, and how it can transform the way we build web applications.

Isomorphic JavaScript refers to the practice of writing JavaScript code that can be executed both on the server-side and the client-side of a web application. Traditionally, web applications have used two distinct approaches for rendering content:

`Server-Side Rendering (SSR):` In SSR, the server generates the HTML content for a web page and sends it to the client's browser. This approach is well-suited for SEO (Search Engine Optimization) because search engines can easily crawl and index the content. However, it often results in slower initial page loads.

`Client-Side Rendering (CSR):` In CSR, the browser downloads a minimal HTML document and then relies on JavaScript to render the content dynamically. This approach can provide a smoother user experience after the initial load but may have SEO challenges.

Isomorphic JavaScript combines the best of both worlds by allowing developers to use a single codebase that can render content on the server and subsequently enhance it on the client. This approach helps improve performance, SEO, and the overall user experience.

**Advantages of Isomorphic JavaScript**

1. `Improved Performance`: Isomorphic JavaScript can significantly reduce the time it takes to display content to users. By rendering pages on the server and sending pre-rendered HTML to the client, you can achieve faster initial page loads. This leads to better perceived performance and a more responsive user interface.

2. `SEO-Friendly`: Search engines often struggle to index content generated solely by client-side JavaScript. Isomorphic JavaScript, with its server-side rendering capabilities, ensures that search engines can easily crawl and index your web pages. This can lead to improved SEO rankings and increased discoverability. Google claims to execute Javascript and analyse the content for Single Page Applications, but there are other search engines also to be considered.

3. `Code Reusability`: Isomorphic code promotes code reusability between the server and client. This can lead to more efficient development, reduced duplication of logic, and easier maintenance.

Packages like lodash, underscore, axios, yup etc. Are Isomorphic in nature. We can run them on either server or client. Based on the environment they return the same output.

Rendering the few things on the server and hydrating rest of the view in browser enhances performance for sure. But rendering html from a component using a library such as React is not simple and maintainable. Extensive testing is required so that no server side code leaks into the client. Debugging may also prove to be difficult. It all depends on the use case and requirement of the application. But surely Node.js has this advantage of having to use the same language on server and client that no other backend framework has.

## Node.js Async Programming Styles

**Callbacks**

Node.js is Asynchronous because of callbacks. As Node.js is event driven, status of tasks are maintained using events. On completion of a task respective callback is fired. This enables for efficient concurrent processing. Callbacks are queued and processed using Event Loop.

`Functions` in Javascript are `First Class Citizens`. Meaning, we can store functions into variables and pass them arguments to other functions. This behaviour of Javascript allows us to pass callback functions to main functions, where is the expectation is to run the callback on task completion.

Callbacks allow us to process the data returned from the main function or handle errors. Callbacks get 2 parameters, first `error` and then `data`. We can check for error variable and handle it.

Function that take in or return other functions as arguments are called as `Higher Order Functions`.

```javascript
function doSomethingAsync(callback) {
  setTimeout(function () {
    console.log("Task completed!");
    callback();
  }, 1000);
}
function onComplete(error, data) {
  console.log("All tasks are done!");
}
doSomethingAsync(onComplete);
```

Output:

```bash +@output
Task completed!
All tasks are done!
```

### Callback Hell

Callback hell is a situation that arises in Node.js and JavaScript when dealing with deeply nested or chained callbacks. This occurs when you have multiple asynchronous operations that depend on the results of previous operations, leading to code that is difficult to read, maintain, and reason about. Callback hell can make your code look like a pyramid of nested callback functions, which can be challenging to work with. Let's illustrate callback hell with an example:

```js
fs.readFile("file1.txt", "utf8", function (err, data1) {
  if (err) {
    handleError(err);
  } else {
    fs.readFile("file2.txt", "utf8", function (err, data2) {
      if (err) {
        handleError(err);
      } else {
        fs.readFile("file3.txt", "utf8", function (err, data3) {
          if (err) {
            handleError(err);
          } else {
            // Perform some more operations...
          }
        });
      }
    });
  }
});

function handleError(err) {
  console.error("An error occurred:", err);
}
```

We use the fs module to read three files sequentially: file1.txt, file2.txt, and file3.txt. For each file read operation, we have a nested callback function to handle the file data or errors. If there are errors in any of the file read operations, we call the handleError function.

Callback hell becomes problematic as more asynchronous operations are added, leading to deeper nesting and making the code less maintainable and error-prone. To mitigate callback hell, you can employ various techniques:

1. Modularization: Break down your code into smaller, reusable functions. This promotes a more structured and readable codebase.

2. Named Functions: Use named functions for your callback handlers instead of anonymous functions. This can make your code more self-documenting and easier to follow.

3. Control Flow Libraries: Consider using control flow libraries like async.js or Promises to manage asynchronous operations in a more organized and linear way.

Here's an example using Promises to mitigate callback hell. We will use the promise based fs module

```js
const fs = require("node:fs/promises");

(async function readFile() {
  const file = "file.txt";
  try {
    const data1 = await fs.readFile(file, "utf-8");
    const data2 = await fs.readFile(file, "utf-8");
    const data3 = await fs.readFile(file, "utf-8");
    console.log("data1", data1);
    console.log("data2", data2);
    console.log("data3", data3);
  } catch (error) {
    console.log("Error", error);
  }
})();
```

### Promises

Promises in JavaScript are a core feature for handling asynchronous operations. They provide a cleaner and more structured way to work with asynchronous code compared to traditional callback patterns. Promises represent a value that may not be available yet but will be resolved at some point in the future, either successfully with a value or unsuccessfully with an error.

**Creating a Promise:**

You can create a Promise using the Promise constructor. It takes a function with two parameters: `resolve` and `reject`.

```js
// Creating a simple promise
const myPromise = new Promise((resolve, reject) => {
  setTimeout(() => {
    const success = true;
    if (success) {
      resolve("Success!");
    } else {
      reject("Error!");
    }
  }, 1000);
});

myPromise
  .then((result) => {
    console.log(result); // Success!
  })
  .catch((error) => {
    console.error(error); // Error!
  });
```

- `resolve` is a function used to fulfill the promise with a value.
- `reject` is a function used to reject the promise with an error.

**Promise States:**

A Promise can be in one of three states:

1. `Pending:` Initial state, neither fulfilled nor rejected.

2. `Fulfilled (Resolved):` The asynchronous operation completed successfully, and the promise holds a resolved value.

3. `Rejected:` The asynchronous operation encountered an error, and the promise holds a rejection reason.

**Chaining Promises:**

Promises can be chained using `.then()` and `.catch()` methods. .then() is used for handling the successful resolution of a promise, and .catch() is used for handling errors.

Promises can also be chained to perform a sequence of asynchronous operations:

```js
// Chaining promises
function asyncTask1() {
  return new Promise((resolve) => {
    setTimeout(() => {
      resolve("Task 1 completed");
    }, 1000);
  });
}

function asyncTask2(result) {
  return new Promise((resolve) => {
    setTimeout(() => {
      resolve(`${result}, Task 2 completed`);
    }, 1000);
  });
}

asyncTask1()
  .then((result1) => {
    return asyncTask2(result1);
  })
  .then((result2) => {
    console.log(result2); // Task 1 completed, Task 2 completed
  })
  .catch((error) => {
    console.error(error);
  });
```

**Promise.all and Promise.race:**

- `Promise.all():` Accepts an array of promises and returns a new promise that resolves when all promises in the array have resolved. If any promise is rejected, the resulting promise is rejected.

```js
// Using Promise.all
const promise1 = Promise.resolve("Promise 1");
const promise2 = Promise.resolve("Promise 2");
const promise3 = Promise.resolve("Promise 3");

Promise.all([promise1, promise2, promise3])
  .then((results) => {
    console.log(results); // ["Promise 1", "Promise 2", "Promise 3"]
  })
  .catch((error) => {
    console.error(error);
  });
```

- `Promise.race():` Accepts an array of promises and returns a new promise that resolves or rejects as soon as the first promise in the array settles (either resolves or rejects).

```js
// Using Promise.race
const promise1 = new Promise((resolve) =>
  setTimeout(() => resolve("Promise 1"), 1000)
);
const promise2 = new Promise((resolve) =>
  setTimeout(() => resolve("Promise 2"), 500)
);

Promise.race([promise1, promise2])
  .then((result) => {
    console.log(result); // Promise 2 (since it resolves first)
  })
  .catch((error) => {
    console.error(error);
  });
```

**Error Handling:**

Promises provide a structured way to handle errors. You can use .catch() at the end of a promise chain to handle errors globally within that chain.

```js
// Error handling with promises
function asyncTask() {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      const success = false;
      if (success) {
        resolve("Success!");
      } else {
        reject("Error!");
      }
    }, 1000);
  });
}

asyncTask()
  .then((result) => {
    console.log(result);
  })
  .catch((error) => {
    console.error(error); // Error!
  });
```

**Promises vs. Callbacks:**

Promises offer several advantages over traditional callback patterns:

- `Readability:` Promises provide a more structured and readable way to work with asynchronous code, avoiding callback hell.

- `Error Handling:` Promises centralize error handling with .catch(), making it easier to handle and propagate errors.

- `Composition:` Promises can be easily composed and chained to perform sequential or parallel operations.

- `Abstraction:` Promises abstract away the details of the asynchronous operation, providing a clear separation of concerns.

### Async/Await

Async/await is a powerful feature in JavaScript for managing asynchronous code. It allows you to write asynchronous code in a more synchronous-looking style, making it easier to read and reason about.

Async/await is built on top of Promises, and it simplifies working with asynchronous operations. It consists of two main keywords:

- `async:` Used before a function declaration to indicate that the function contains asynchronous code and will return a Promise.

- `await:` Used inside an async function to pause the execution until a Promise is resolved. It can only be used inside async functions.

Inside an async function, you can use await to pause the execution until a Promise is resolved.

```js
async function fetchData() {
  try {
    const response = await fetch("https://api.example.com/data");
    if (!response.ok) {
      throw new Error("Failed to fetch data");
    }
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

fetchData();
```

We can handle errors in Async/Await using try/catch blocks. Initiate the promise inside try block. If promises rejects it'll be caught in the catch block.

Async/await allows you to perform parallel asynchronous operations. You can use Promise.all to await multiple Promises concurrently:

```js
async function fetchDataParallel() {
  try {
    const [data1, data2] = await Promise.all([
      fetch("https://api.example.com/data1").then((response) =>
        response.json()
      ),
      fetch("https://api.example.com/data2").then((response) =>
        response.json()
      ),
    ]);
    console.log(data1, data2);
  } catch (error) {
    console.error(error);
  }
}

fetchDataParallel();
```

### Node.js Patterns

Node.js design patterns are reusable solutions to common problems encountered in Node.js applications. They help developers write code that is more maintainable, efficient, and scalable. In this discussion, we'll explore some common Node.js design patterns in detail, along with examples.

**Singleton Pattern**

The Singleton pattern ensures that a class has only one instance and provides a global point of access to that instance. That means we cannot create multiple instances - just one. It's often used for managing shared resources, such as database connections or configuration settings, to prevent unnecessary duplication.

```javascript
class DatabaseConnection {
  constructor() {
    this.databaseConnection = "dummytext";
  }

  getNewDBConnection() {
    return this.databaseConnection;
  }
}

module.exports = new DatabaseConnection();
```

In the above code we see that the instance of the class is exported. That means, we cannot create more instances of the class. We can only use this single instance. This type of implementation is required where in we have to share the same data through out our application. For example database connection or methods to connect or disconnet. Or a datastore in UI application, only a single instance of datastore should be present, only then we can update and retrieve data to and from multiple components.

> Note: Node.js caches the modules it imported. Even if we import the above database connection module twice. Node.js doesn't import the second time and picks up module from its cache.

**Factory Pattern**

The Factory Design Pattern allows us to define an interface or abstract class used to create an object. We then use the interface/abstract class to instantiate different objects.

Consider an application where we have to create and use all types of vehicles. There are motor vehicles (cars, buses, trucks, motorcycles), railed vehicles (trains, trams), aircraft (airplanes, helicopters), and watercraft (ships, boats). Thus, instead of creating instances by calling the constructor of each class individually, we can implement the Factory pattern as follows:

```javascript
import Motorvehicle from "./Motorvehicle";
import Aircraft from "./Aircraf";
import Railvehicle from "./Railvehicle";

const VehicleFactory = (type, make, model, year) => {
  if (type === car) {
    return new Motorvehicle("car", make, model, year);
  } else if (type === airplane) {
    return new Aircraft("airplane", make, model, year);
  } else if (type === helicopter) {
    return new Aircraft("helicopter", make, model, year);
  } else {
    return new Railvehicle("train", make, model, year);
  }
};

module.exports = VehicleFactory;
```

The benefit of using the Factory design pattern is that it decouples the objects' constructions from the objects themselves. You can also introduce new objects into your application without breaking existing code. Lastly, it helps you organize your code better because all the code related to creating instances is in one place.

- Factory pattern provides an interface/abstract class for creating objects.
- You can create different objects by using the same interface/abstract class.
- It improves the structure of the code and makes it easier to maintain it.

**Builder Pattern**

The Builder design pattern allows us to separate the construction of objects from their representation. Thus, it simplifies the code that creates complex objects. It might be overkill with simple objects, but with complex objects, it simplifies creating them.

To help you with understanding this design pattern, let's think of an example. Let's say we want to build cars. In this example, we would have the Car and CarBuilder classes.

```javascript
class Car {
  constructor(make, model, year, isForSale = true, isInStock = false) {
    this.make = make;
    this.model = model;
    this.year = year;
    this.isForSale = isForSale;
    this.isInStock = isInStock;
  }

  toString() {
    return console.log(JSON.stringify(this));
  }
}

class CarBuilder {
  constructor(make, model, year) {
    this.make = make;
    this.model = model;
    this.year = year;
  }

  notForSale() {
    this.isForSale = false;

    return this;
  }

  addInStock() {
    this.isInStock = true;

    return this;
  }

  build() {
    return new Car(
      this.make,
      this.model,
      this.year,
      this.isForSale,
      this.isInStock
    );
  }
}

module.exports = CarBuilder;
```

Now we create cars using the CarBuilder class instead of the Car class. We do it as follows:

```js
const CarBuilder = require("./CarBuilder");

const bmw = new CarBuilder("bmw", "x6", 2020).addInStock().build();
const audi = new CarBuilder("audi", "a8", 2021).notForSale().build();
const mercedes = new CarBuilder("mercedes-benz", "c-class", 2019).build();
```

Using the Builder design pattern makes the creation of complex objects less prone to errors because you can easily understand what each parameter does. For contrast, here is how we would create cars without the CarBuilder class:

```js
const bmw = new CarBuilder("bmw", "x6", 2020, true, true);
```

You can see it can become confusing. What do those two boolean values ("true") mean? Now imagine the object is more complex; creating the object would be confusing, and the chances of introducing errors would be higher.

Thus, the Builder design pattern is useful to separate the creation and representation of complex objects.

**Facade Pattern**

Facade pattern is used to provide an abstraction over and implementation and provide a clean api to its consumers. By separate the implementation logic its easy to make modifications in the future because we just have to change in place. Also providing all the defaults helps us in removing duplication where ever the object of this class is used.

```js
function getUsers() {
  return fetch("https://jsonplaceholder.typicode.com/users", {
    method: "GET",
    headers: { "Content-Type": "application/json" },
  }).then((res) => res.json());
}

function getUserPosts(userId) {
  return fetch(`https://jsonplaceholder.typicode.com/posts?userId=${userId}`, {
    method: "GET",
    headers: { "Content-Type": "application/json" },
  }).then((res) => res.json());
}

getUsers().then((users) => {
  users.forEach((user) => {
    getUserPosts(user.id).then((posts) => {
      console.log(user.name);
      console.log(posts.length);
    });
  });
});
```

In the above code we are making an api call and fetching all the users and their number of posts. We see that in the fetch function method and headers are duplicated. Lets see how we can improve this with Facade Pattern.

```js
function getUsers() {
  return getFetch("https://jsonplaceholder.typicode.com/users");
}

function getUserPosts(userId) {
  return getFetch("https://jsonplaceholder.typicode.com/posts", {
    userId: userId,
  });
}

getUsers().then((users) => {
  users.forEach((user) => {
    getUserPosts(user.id).then((posts) => {
      console.log(user.name);
      console.log(posts.length);
    });
  });
});

function getFetch(url, params = {}) {
  const queryString = Object.entries(params)
    .map((param) => {
      return `${param[0]}=${param[1]}`;
    })
    .join("&");
  return fetch(`${url}?${queryString}`, {
    method: "GET",
    headers: { "Content-Type": "application/json" },
  }).then((res) => res.json());
}
```

Whenever we feel we are repeting the logic, its better to separate and provide a simple and flexible api to interact with it. This helps us to make changes to that implementation in the future and also delivers a standard behaviour which helps in dubugging aswell.

## CommonJs and Modular Node Application

### Modules

Modularisation is splitting the code into files(modules). This enables us to write maintainable code and reuse the logic instead of repeating the code. We import a module in Node using the `require` function.

`CommonJs` is a modular standard that Node.js adopted when it rolled out initially. `Modules` are nothing but files or a collection a files that export its functionality. Lets look at an example to see why we need modules.

```js index.js
const add = (a, b) => {
  return a + b;
};
const subtract = (a, b) => {
  return a - b;
};
console.log("add: ", add(1, 2));
console.log("subtraction: ", subtract(1, 2));
```

We have 2 functions here with add and subtract functionality. Its not very maintainable or readable to have all the logic within a single file. Lets group the common logic and modularise it. Lets create a new file `arithmetic.js` and move the add and subtract functions. Just moving the code into a separate file doesn't enable us to use that inside our index.js file. We have to mention what all functionality of variables we are exporting. we do that by assigning variable to `module.exports` object.

```js arithmetic.js
const add = (a, b) => {
  return a + b;
};
const subtract = (a, b) => {
  return a - b;
};
module.exports = { add, subtract };
```

Now we can import all the functionality present inside a module using the `require` keyword.

```js index.js
const arithmetic = require("./arithmetic.js");

console.log("add: ", arithmetic.add(1, 2));
console.log("subtraction: ", arithmetic.subtract(1, 2));
```

Output:

```bash +@output
add:  3
subtraction:  -1
```

We imported the entire object that was being exported from arithmetic.js file. So `arithmetic` variable is an object with 2 keys (`add`, `subtract`). We use them by using the `dot` notation on `arithmetic`.

> Note: While importing we need not specify the file extension (.js). Node.js looks for appends .js and imports the file. If you are working with other file type aswell like `.json`, `.ts`. Its a good idea to import by using the file extension when you have files with different extension have the same file name. For example, if you have 2 files `data.js` and `data.json`, while importing json from data.json its good to have .json extension in require statement.

**Module scope**

```js module1.js
const language = "Javascript";
console.log(language);
```

```js module2.js
const language = "Python";
console.log(language);
```

```js index.js
require("./module1.js");
require("./module2.js");
```

Output:

```bash +@output
Javascript
Python
```

After running `index.js` file, we see the above output. Even though same variable names are used in these 2 modules. They do not concflict in import. This is exactly how modules should work. Reuse of variable names should not conflict.

> `require` wraps the module inside of an IIFE(Immediately Invoked Function Expression) which makes variables function scoped. So there wont be any conflicts.

**Module Wrapper**

We saw that each module is wrapped inside of an IIFE. This IIFE gets 5 parameters injected by Node.js. These parameters are accessible inside each module being imported.

- `exports:` reference to `exports` property of `module` object.
- `require:` This function is used to import other modules. When you use require, Node.js looks for the specified module, executes its code (if not executed before), and returns the module's exports object.
- `module:` This object represents the current module and contains information about the module, such as its filename and exports. Its property `exports` is injected as another standalone parameter into module being imported.
- `__filename:` This variable contains the absolute path to the current module's file.
- `__dirname:` This variable contains the absolute path to the directory where the current module is located.

**Module Caching**

```js -index.js
const language1 = require("./module");
console.log(language1.getName());
language1.setName("Python");
console.log(language1.getName());

const language2 = require("./module");
console.log(language2.getName());
```

```js +module.js
class Language {
  constructor(name) {
    this.name = name;
  }
  getName() {
    return this.name;
  }
  setName(name) {
    this.name = name;
  }
}

module.exports = new Language("JavaScript");
```

Output:

```bash +@output
JavaScript
Python
Python
```

Above code in `index.js` we require the object exported from `module.js` file. We get the name and then again set the name. Second console log shows that the name was updated. When we require the module again, and logging the name, it should be `Javascript`. Because we are importing the new object. But this doesn't happen. Instead we see `Python` being logged to console. This is because of module caching. `require` function has a property `cache` which stores information about modules imported. Once a module is imported it is not re imported.

**Export Patterns**

We can export functionalities from a module in different ways. Lets see them.

```js
const add = (a,b) => V{
  return a + b;
}

module.exports = add
```

We import into out index.js file and use the method directly.

```js
const add = require("./math.js");
console.log(add(1, 2)); // 3
```

```js
module.exports = (a, b) => {
  return a + b;
};
```

In the above snippet instead of assigning the function to a variable and then exporting, we directly assign the function to `module.exports`.

```js
const add = (a,b) => V{
  return a + b;
}
const subtract = (a,b) => V{
  return a - b;
}

module.exports = {add, subtract};
```

If there are more functions are properties we want to export then we can do so as an object. We can import the object and use a dot operator to access the properties. Or destructure and use the properties directly.

```js
const math = require("./math.js");

console.log(math.add(1, 2)); // 3
console.log(math.subtract(1, 2)); // -1
```

```js
const { add, subtract } = require("./math.js");

console.log(add(1, 2)); // 3
console.log(subtract(1, 2)); // -1
```

> Note: Always assign functions or properties to `module.exports` and not `exports` directly. If we assign an object to `module.exports` import works fine. If the same is done to `exports` import breaks. We discussed `exports` is a reference to `module.exports`. When exporting `exports` from a module the reference breaks and `module.exports` becomes an empty object.

**ES Modules**

ECMAScript (ES) Modules, also known as ES6 Modules or ES Modules, are a standardized system for organizing and sharing JavaScript code in a modular and efficient way. ES Modules have been introduced as part of the ECMAScript 6 (ES6) specification and are now widely supported in Node.js, making it easier to write modular and maintainable code.

ES Modules offer several advantages for organizing and sharing JavaScript code:

1. `Explicit Imports and Exports:` With ES Modules, you explicitly define which variables, functions, or classes you want to import and export, improving code readability and reducing ambiguity.

2. `Improved Performance:` ES Modules are statically analyzed, which enables tools to perform optimizations like tree-shaking (removing unused code) for better performance.

3. `Browser Compatibility:` ES Modules are supported in modern browsers, making it possible to share code between the server and the client.

Importing and Exporting in ES Modules:

`Exporting:` To make variables, functions, or classes available for use in other modules, you use the export keyword.

```js math.js
// Export a constant
export const PI = 3.14159265359;

// Export a function
export function square(x) {
  return x * x;
}
```

`Importing:` To use variables, functions, or classes from other modules, you use the import keyword.

```js index.js
// Import named exports
import { PI, square } from "./math.js";

console.log(`The value of PI is ${PI}`);
console.log(`The square of 4 is ${square(4)}`);
```

Output:

```bash +@output
The value of PI is 3.14159265359
The square of 4 is 16
```

### Type of Modules

**Core Modules**

Core modules are built-in modules provided by Node.js. They include commonly used functionalities, such as file system operations, networking, and utilities. You can use core modules by requiring them using require. Examples of core modules include fs (file system), http (HTTP server/client), os (operating system), and path (path manipulation).

```js
const fs = require("fs");
const http = require("http");
```

**Local Modules**

Local modules are modules that you create and store in your project directory. They allow you to organize your codebase into smaller, reusable files. You can require local modules using relative paths. Local modules are an essential part of structuring a Node.js application, as they promote code reusability and maintainability.

```js
const myModule = require("./myModule");
```

**Third-Party Modules**

Third-party modules are modules created by other developers and made available through the Node Package Manager (NPM). These modules extend Node.js's functionality and can be easily integrated into your project. To use a third-party module, you first need to install it using npm install and then require it in your code. Third-party modules cover a wide range of functionalities, from web frameworks like Express to utility libraries like Lodash.

```js
const express = require("express");
const lodash = require("lodash");
```

### Core modules: OS, Events, Filesystem and Network

Lets discuss few core modules.

**Os Module**

The os module in Node.js provides a way to access various operating system-related information and functionalities. It can be used to retrieve data about the computer's operating system, network interfaces, and system resources

Few things we can do using OS Module

- Obtain information about the underlying operating system.
- Retrieve the system's uptime in seconds.
- Retrieve information about the CPU, such as the number of CPU cores and architecture.
- Access memory-related information, such as total memory and free memory.
- Retrieve information about network interfaces on the system.
- Access information about the currently logged-in user.

```js
const os = require("os");

// Example 1: Getting OS Information
console.log("OS Type:", os.type());
console.log("Platform:", os.platform());
console.log("OS Release:", os.release());
console.log("Hostname:", os.hostname());

// Example 2: Retrieving System Uptime
console.log("Uptime (seconds):", os.uptime());

// Example 3: Retrieving CPU Information
console.log("CPU Cores:", os.cpus().length);
console.log("CPU Architecture:", os.arch());
console.log("CPU Model:", os.cpus()[0].model);

// Example 4: Retrieving Memory Information
console.log("Total Memory (bytes):", os.totalmem());
console.log("Free Memory (bytes):", os.freemem());

// Example 5: Retrieving Network Interfaces
const networkInterfaces = os.networkInterfaces();
console.log("Network Interfaces:", networkInterfaces);

// Example 6: Retrieving User Information
console.log("User Home Directory:", os.homedir());
console.log("Username:", os.userInfo().username);
```

**Events Module**

The events module in Node.js provides a framework for implementing and working with events and event emitters. Events are a fundamental part of many applications, allowing you to create custom events and handle them asynchronously.

The events module provides two core classes: EventEmitter and Event. The EventEmitter class serves as the foundation for creating event emitters and handling events. Event emitters are objects that emit named events, and you can register functions (event listeners) to be called when those events are emitted.

Here are the key components of the events module:

- EventEmitter: The core class that allows you to emit events and register event listeners.
- Event: Objects that represent events and their associated data (optional).

1. Creating and Emitting Custom Events:

```js
const EventEmitter = require("events");

// Create a custom event emitter
class MyEmitter extends EventEmitter {}

const myEmitter = new MyEmitter();

// Register an event listener
myEmitter.on("myEvent", () => {
  console.log("Custom event emitted");
});

// Emit the custom event
myEmitter.emit("myEvent");
```

In the above example, we import the events module and create a custom event emitter class, MyEmitter, which inherits from EventEmitter.
Register an event listener for the 'myEvent' event using the on method.
Emit the custom event using the emit method.

2. Passing Data with Events:

```js
const EventEmitter = require("events");

class MyEmitter extends EventEmitter {}

const myEmitter = new MyEmitter();

myEmitter.on("dataEvent", (data) => {
  console.log("Received data:", data);
});

myEmitter.emit("dataEvent", { message: "Hello, World!" });
```

Here, when emitting the 'dataEvent', we pass an object containing a message as data to the event listener.

3. Handling Error Events:

The EventEmitter class also provides a special 'error' event that can be used for error handling.

```js
const EventEmitter = require("events");

class MyEmitter extends EventEmitter {}

const myEmitter = new MyEmitter();

myEmitter.on("error", (err) => {
  console.error("Error:", err.message);
});

myEmitter.emit("error", new Error("Something went wrong"));
```

In this example, we register an event listener for the 'error' event and emit an error event with an Error object

4. One-Time Event Listeners:

You can register one-time event listeners using the once method. These listeners are automatically removed after being called once.

```js
const EventEmitter = require("events");

class MyEmitter extends EventEmitter {}

const myEmitter = new MyEmitter();

myEmitter.once("onceEvent", () => {
  console.log("This listener will only be called once.");
});

myEmitter.emit("onceEvent");
myEmitter.emit("onceEvent"); // This won't trigger the listener again
```

5. Removing Event Listeners:

You can remove event listeners using the removeListener method.

```js
const EventEmitter = require("events");

class MyEmitter extends EventEmitter {}

const myEmitter = new MyEmitter();

function eventHandler() {
  console.log("Event handler called");
}

myEmitter.on("removeEvent", eventHandler);

myEmitter.emit("removeEvent");

myEmitter.removeListener("removeEvent", eventHandler);

myEmitter.emit("removeEvent"); // Event handler won't be called
```

In this example, we add an event listener with on, remove it with removeListener, and then verify that it no longer triggers.

EventEmitter Best Practices:

- Always handle errors. Use the error event for error handling.
- Use meaningful event names.
- Be cautious with memory management when registering many listeners for the same event.

**Path Module**

The path module in Node.js is a core module that provides utilities for working with file and directory paths. It helps in ensuring that your code remains platform-independent by handling path-related operations in a cross-platform manner, regardless of the underlying operating system.

1. path.join: The path.join function joins one or more path segments together using the appropriate separator for the current operating system. It automatically handles the differences between forward slashes (/) and backslashes (\) on Windows and Unix-based systems.

2. path.resolve: The path.resolve function resolves an absolute path from the given arguments. It processes each argument from right to left, building the path from the root directory.

3. path.basename: The path.basename function returns the last portion of a path. Optionally, you can provide an extension to remove it from the filename.

4. path.dirname: The path.dirname function returns the directory name of a path.

5. path.extname: The path.extname function returns the extension of a path, including the dot (.).

6. path.parse: The path.parse function returns an object containing various components of a path, such as root, dir, base, name, and ext.

Few examples using path module

```js
const path = require("path");

// Joining path segments
const fullPath = path.join(__dirname, "subdir", "file.txt");
console.log("Full path:", fullPath);

// Resolving an absolute path
const resolvedPath = path.resolve(
  "/home/user",
  "projects",
  "myapp",
  "file.txt"
);
console.log("Resolved path:", resolvedPath);

// Getting the file name and directory name
const fileName = path.basename("/path/to/file.txt");
console.log("File name:", fileName); // file.txt

const dirName = path.dirname("/path/to/file.txt");
console.log("Directory name:", dirName); // /path/to

// Getting the file extension
const ext = path.extname("/path/to/file.txt");
console.log("Extension:", ext); // .txt

// Parsing a path
const pathInfo = path.parse("/path/to/file.txt");
console.log("Path components:", pathInfo);
```

Output:

```bash +@output
Resolved path: C:\home\user\projects\myapp\file.txt
File name: file.txt
Directory name: /path/to
Extension: .txt
Path components: {
  root: '/',
  dir: '/path/to',
  base: 'file.txt',
  ext: '.txt',
  name: 'file'
}
```

### node_modules folder

The node_modules folder in a Node.js project plays a crucial role in managing dependencies. It contains third-party packages and libraries that your project depends on. When you install a third party package it is saved inside `node_modules` folder. You can import the functionalities of that package using `require` keyword and using it inside your project.

**Purpose of the node_modules Folder**

1. `Dependency Management:` The primary purpose of the node_modules folder is to manage project dependencies. When you install third-party packages or libraries using a package manager like npm (Node Package Manager) or Yarn, these packages are downloaded and stored in the node_modules directory.

2. `Isolation:` Each project typically has its own node_modules folder. This isolation ensures that different projects can have different dependencies with potentially different versions without conflicting with each other. It also means that your project's dependencies won't interfere with the global Node.js environment.

**How the node_modules Folder Works**

1. `Dependency Resolution:` When you require a module in your JavaScript code using require('module-name'), Node.js will search for the module-name package in the current project's node_modules folder. If it's not found there, Node.js will traverse up the directory tree, searching in parent directories until it finds a node_modules folder with the required package or reaches the root directory.

2. `Package.json and package-lock.json:` Dependencies are usually declared in the package.json file of your project. When you install or update packages using npm or Yarn, these tools will automatically update the package.json file and create or update a package-lock.json file (or yarn.lock in the case of Yarn). These lock files ensure that your project consistently uses the same versions of packages, avoiding unexpected changes when you or your team members work on the project.

3. `Nested Dependencies:` A package can have its own dependencies listed in its package.json file. These are called "nested dependencies." When you install a package, its nested dependencies are also installed in your project's node_modules folder. This ensures that the entire dependency tree is available for your project.

4. `Scoped Packages:` Scoped packages, which are often used for packages belonging to a specific organization or user, have a directory structure within the node_modules folder that includes the scope name (e.g., @organization/package). Scoped packages help prevent naming conflicts.

**Best Practices**

1. `Use a Package Manager:` Always use a package manager like npm or Yarn to manage your project's dependencies. This ensures consistent and reproducible builds.

2. `Declare Dependencies:` Keep your package.json file up to date with accurate dependencies and versions.

3. `Avoid Modifying node_modules Directly:` Don't manually add or remove files in the node_modules folder, as this can lead to inconsistencies and conflicts.

4. `Use Lock Files:` Lock files like package-lock.json or yarn.lock help ensure that everyone working on the project uses the same versions of dependencies.

5. `Regularly Update Dependencies:` Periodically update your project's dependencies to benefit from bug fixes, security updates, and new features. Use tools like npm outdated or yarn outdated to check for updates.

## NPM Getting Started

npm (Node Package Manager) is a powerful and widely used package manager for JavaScript and Node.js projects. It simplifies the process of managing and sharing code and dependencies, making it an essential tool for modern web and Node.js development

### Why npm?

1. `Dependency Management:` npm simplifies the process of managing project dependencies. It allows you to specify and track the packages your project relies on, making it easier to maintain and share your code.

2. `Package Discovery:` npm's online repository contains thousands of packages created by the open-source community. You can easily find and use packages for various tasks, from front-end libraries to server-side frameworks.

3. `Version Control:` npm provides version control for packages, allowing you to specify the exact versions or version ranges your project requires. This ensures consistency across different environments and team members.

4. `Scripts and Automation:` npm includes a script runner that lets you define and run custom tasks in your project. This is useful for automating build processes, testing, and other common development tasks.

5. `Publishing Packages:` If you develop reusable code, npm allows you to publish your packages to the npm registry, making them accessible to other developers worldwide.

**Key npm Components:**

1. `npm Registry:` The npm registry is a centralized online database of JavaScript packages. When you install a package using npm install package-name, npm fetches the package from the registry and installs it in your project's node_modules directory.

2. `npm Command-Line Interface (CLI):` The npm CLI is a command-line tool that provides commands for installing, updating, publishing, and managing packages. Common commands include npm install, npm publish, npm update, and npm run.

3. `package.json:` The package.json file is a manifest for your project. It includes metadata about your project, such as its name, version, dependencies, and scripts. Developers can share this file to ensure that others can set up the project correctly.

4. `package-lock.json:` The package-lock.json file is automatically generated by npm to lock down the specific versions of dependencies used in a project. This ensures consistency among team members and across different environments.

### npm Configuration

npm can be configured using the .npmrc file in your user's home directory or in your project directory. Configuration options can include registry URLs, authentication tokens, proxy settings, and more. These configurations help npm work smoothly within your organization or on your local machine.

Here is a sample .npmrc file

```text
# Set the registry to the default npm registry (https://registry.npmjs.org/)
registry=https://registry.npmjs.org/

# Define a custom registry (uncomment and modify if needed)
# registry=https://custom-registry-url.com/

# Specify a proxy server for outgoing HTTP requests (uncomment and modify if needed)
# proxy=http://your-proxy-server-url.com:8080

# Specify a proxy server for outgoing HTTPS requests (uncomment and modify if needed)
# https-proxy=http://your-proxy-server-url.com:8080

# Set the location for globally installed packages
prefix=/usr/local

# Disable progress bar during package installation
progress=false

# Skip optional dependency installation
optional=false

# Define a custom user agent for npm requests (uncomment and modify if needed)
# user-agent=my-custom-user-agent

# Specify the default package scope (uncomment and modify if needed)
# scope=myorg

# Save exact versions in package.json (recommended for reproducible builds)
save-exact=true

# Log verbosity (silent, error, warn, info, verbose, silly)
loglevel=info
```

### package.json

`package.json` file serves as a manifest for your project, documenting various aspects, including project metadata, dependencies, scripts, and more. A package.json file is a JSON (JavaScript Object Notation) file that provides essential information about a Node.js project. It includes details like project name, version, author, license, and most importantly, a list of dependencies required to run the project.

Here's a sample package.json file with explanations of the important configurations:

```json
{
  "name": "my-node-project", // Name of your project
  "version": "1.0.0", // Project version
  "description": "My Node.js app", // Project description
  "main": "index.js", // Entry point for the application
  "scripts": {
    "start": "node index.js", // Custom scripts for running the app
    "test": "mocha tests/**/*.js" // Custom scripts for testing
  },
  "keywords": ["node", "example"], // Keywords related to your project
  "author": "Your Name", // Author's name
  "license": "MIT", // License type
  "dependencies": {
    "express": "^4.17.1", // Dependencies required for the app
    "axios": "^0.21.4"
  },
  "devDependencies": {
    "mocha": "^9.1.0", // Development dependencies (e.g., testing tools)
    "chai": "^4.3.4"
  }
}
```

**Important package.json Configurations:**

1. `name:` The name of your project. It should be unique on the npm registry. The convention is to use lowercase letters and hyphens for names (e.g., "my-node-project").

2. `version:` The version number of your project. Follow semantic versioning (semver) guidelines, which typically consist of three numbers (e.g., "1.0.0" or "3.2.1"). Semver defines how versions should be incremented based on changes.

3. `description:` A brief description of your project, helping others understand its purpose and functionality.

4. `main:` The entry point for your application, usually a JavaScript file (e.g., "index.js"). This is the file that will be executed when your project is run.

5. `scripts:` Defines custom scripts for various tasks, such as starting the application or running tests. These scripts can be executed using npm run script-name (e.g., npm run start or npm run test).

6. `keywords:` An array of keywords related to your project. These keywords help others discover your project when searching for similar tools or libraries.

7. `author:` The name of the project's author or maintainers.

8. `license:` The type of license under which your project is distributed. Common licenses include "MIT," "Apache-2.0," and "GPL-3.0."

9. `dependencies:` A list of runtime dependencies required for your project to work. Dependencies are specified as key-value pairs, where the key is the package name, and the value is the version or version range required. npm will automatically install these packages when someone else runs npm install in your project.

10. `devDependencies:` Similar to dependencies, but for development-specific dependencies like testing libraries or build tools. These dependencies are typically not needed in a production environment and can be installed separately using npm install --dev.

**Generating a package.json File:**

You can generate a package.json file interactively by running `npm init` command in your project's directory. npm will prompt you with questions to fill in the fields of the package.json file. You can also use the -y or --yes flag to accept all the default values. `npm init -y`. This command will create a package.json file with minimal information, and you can edit it later to add more details.

**npm Commands**

- `npm install package-name:` Installs a package and its dependencies.

- `npm install -g package-name:` Installs a package globally (useful for command-line tools).

- `npm init:`` Creates a new package.json file interactively.

- `npm publish:` Publishes a package to the npm registry.

- `npm search package-name:` Searches for packages in the registry.

- `npm outdated:` Checks for outdated dependencies in your project.

- `npm update package-name:` Updates a package to its latest version.

- `npm run script-name:` Executes a script defined in your package.json file.

- `npm config set key value:` Sets a configuration option.

- `npm cache clean -f:` Clears the npm cache.

### Develop and Production Dependencies\*\*

**1. Development Dependencies (devDependencies):**

Development dependencies, often listed under the devDependencies section in your project's package.json file, are packages and modules that are used during the development and testing phases of your application. They play a crucial role in tasks related to development, testing, and building the application but are not required for the application to run in production.

Common Examples of Dev Dependencies:

1. `Testing Frameworks:` Libraries like Mocha, Jest, or Jasmine are used for writing and running tests.

2. `Linters:` Tools like ESLint or JSHint are used for code linting and style checking to maintain code quality.

3. `Build Tools:` Tools like Webpack, Gulp, or Grunt are used to bundle, minify, or transpile code during development.

4. `Mocking Libraries:` Libraries like Sinon or Nock help create mock objects or simulate API responses during testing.

5. `Documentation Generators:` Tools like JSDoc or ESDoc generate documentation from code comments

Why Use Dev Dependencies?

1. `Development Efficiency:` Dev dependencies streamline the development process, making it easier to write, test, and maintain code.

2. `Code Quality:` Linters and code analysis tools help enforce coding standards and identify potential issues early in the development cycle.

3. `Testing:` Testing frameworks and tools facilitate comprehensive testing, ensuring that the application functions correctly.

4. `Build and Deployment:` Build tools and scripts automate tasks like bundling and minifying code, simplifying deployment.

Installation:

You can install dev dependencies using the npm install --save-dev or npm install -D command. For example:

```bash
npm install --save-dev mocha
```

**2. Production Dependencies (dependencies):**

Production dependencies, listed under the dependencies section in your package.json file, are packages and modules that are essential for your application to run in a production environment. These dependencies are what your application relies on to function correctly when deployed to a production server

Common Examples of Production Dependencies:

1. `Web Frameworks:` Libraries like Express.js, Koa, or Hapi.js provide the core functionality for building web applications.

2. `Database Drivers:` Packages like mongoose (for MongoDB) or pg (for PostgreSQL) are essential for database connectivity.

3. `Authentication Libraries:` Libraries like Passport.js provide authentication strategies for user authentication.

4. `Logging Tools:` Libraries like Winston or Bunyan are used for application logging.

5. `Request Libraries:` Libraries like Axios or node-fetch are used for making HTTP requests to external services or APIs.

Why Use Production Dependencies?

1. `Application Functionality:` Production dependencies provide core functionality for your application to serve its intended purpose.

2. `Reliability:` These dependencies are thoroughly tested and maintained to ensure reliability and security.

3. `Performance:` Production dependencies are optimized for performance, making them suitable for handling production-level traffic.

4. `Security:` Production dependencies receive regular security updates and are generally considered safe for use in production environments.

Installation:

You can install production dependencies using the npm install or npm install --save command. For example:

```bash
npm install express
```

### Global Dependencies

Global modules in Node.js refer to packages or modules that are installed globally on your system, rather than being scoped to a specific project. These modules are accessible from any Node.js project or script you create, regardless of the project's location on your file system. Understanding global modules is essential when working with Node.js, as they enable you to use command-line tools and utilities across different projects without the need for repetitive installations.

**Key Aspects of Global Modules:**

1. `Installation:` Global modules are installed using the -g or --global flag with the npm install command. For example: `npm install -g package-name`. This installs the specified package globally and makes it accessible as a command-line tool.

2. `Usage:` Once installed globally, you can use the global module's command or functionality in any terminal session without needing to install it for each individual project. For example, if you install a package called my-cli-tool, you can use it like this: `my-cli-tool command arguments`. This makes it convenient to run command-line tools or utilities from anywhere in your file system.

3. `Global Module Path:` Global modules are typically stored in a system-specific directory. On Unix-based systems (Linux, macOS), they are stored in the /usr/local/lib/node_modules directory. On Windows, they are stored in C:\Users\<Username>\AppData\Roaming\npm\node_modules. You can check the global module path by running: `npm root -g`.

4. `$PATH Environment Variable:` To use global modules, ensure that the directory containing globally installed modules is in your system's PATH environment variable. This allows the system to locate and execute the command-line tools provided by global modules.

5. `Global Modules vs. Local Modules:` Global modules are different from local modules, which are installed within a specific project's node_modules directory. Local modules are project-specific and are not available globally across all projects.

6. `Updates and Maintenance:` It's essential to keep global modules up-to-date to benefit from bug fixes and new features. You can update global modules using the npm update -g command.

7. `Avoid Overuse:` While global modules are convenient for command-line tools and utilities, it's generally a best practice to keep project-specific dependencies in the node_modules directory of each project. Global modules should be reserved for tools that are genuinely meant to be used across multiple projects.

**Examples of Global Modules:**

Here are some common examples of global modules in Node.js:

1. `Nodemon:` A tool that automatically restarts Node.js applications during development when code changes are detected.

2. `ESLint:` A popular code linter and static analysis tool for identifying and fixing problems in JavaScript code.

**Best Practices:**

- Use global modules sparingly and only for command-line tools and utilities that are genuinely needed across multiple projects.

- Document the global modules your project relies on in your project's README or documentation so that other developers can easily install them.

- Periodically check for updates to global modules and update them as needed to benefit from improvements and security fixes.

### Publishing packages to npm repository

Publishing packages to the npm registry is a fundamental aspect of sharing your JavaScript and Node.js code with the broader developer community. The npm registry is a central repository where you can publish your packages and make them available for others to install and use in their projects.

**Prerequisites:**

Before you publish your package to the npm registry, ensure you have the following:

1. `npm Account:` You need an npm user account. You can create one by running the following command and following the prompts: `npm adduser`.

2. `Package to Publish:` You should have a directory containing your package's code and a package.json file that defines your package's metadata and dependencies.

**Steps to Publish a Package to the npm Registry:**

1. `Verify Your package.json:` Ensure that your package.json file is correctly configured with all the necessary metadata, including the name, version, description, and author fields. Review your package's dependencies and scripts as well.

2. `Versioning:` Follow semantic versioning (semver) guidelines when assigning versions to your package. Use npm version to bump the version number in your package.json file.

```bash
npm version <major|minor|patch>
```

3. `Login to npm:` Before you can publish, you need to log in to your npm account using the npm login command. Provide your npm username, password, and email address when prompted.

```bash
npm login
```

4. `Publish Your Package:` Use the npm publish command to publish your package to the npm registry. This will package your code and metadata and make it available to the public or a selected audience, depending on your npm account settings.

```bash
npm publish
```

6. `Unpublishing (Use with Caution):` Once you publish a package, it's generally considered a best practice not to unpublish it, especially if others depend on it. Unpublishing can break other projects that rely on your package. However, if you must unpublish, you can do so using the npm unpublish command. Keep in mind that there are restrictions on unpublishing versions of a package that are older than 72 hours.

```bash
# Unpublish the package (use with caution)
npm unpublish <package>@<version>
```

### SemVer Versioning Systems

Semantic Versioning, often abbreviated as SemVer, is a versioning system used primarily in the software development industry to manage and communicate changes in software libraries, packages, and applications. This versioning system provides a clear and standardized way of indicating the nature of changes between different versions, helping developers make informed decisions about updating their dependencies.

**Principles of Semantic Versioning:**

Semantic Versioning follows a set of principles to convey meaning about changes in software. These principles include:

1. `Version Format:` A version number consists of three parts: MAJOR.MINOR.PATCH. These parts are separated by periods and represent different aspects of the software's changes.

- `MAJOR` version increment indicates backward-incompatible changes.
- `MINOR` version increment indicates backward-compatible new features.
- `PATCH` version increment indicates backward-compatible bug fixes.

2. `Pre-release and Build Metadata:` Additional information can be appended to versions as pre-release or build metadata. These identifiers are optional and do not affect version precedence. For example, 1.2.3-alpha+001.

**Semantic Versioning Syntax:**

The SemVer versioning system has a straightforward syntax:

- `MAJOR.MINOR.PATCH:` These are numeric values separated by periods. For example, 1.2.3.

- `Pre-release Identifier:` An optional identifier for pre-release versions, typically indicated by a hyphen followed by alphanumeric characters and hyphens (e.g., -beta.1).

- `Build Metadata:` An optional build metadata identifier, typically indicated by a plus sign followed by alphanumeric characters and hyphens (e.g., +001).

**Applying Semantic Versioning:**

Here's how developers typically apply Semantic Versioning to software projects:

1. `MAJOR Version Increment:` When making incompatible changes that require users to modify their code or configurations, increment the MAJOR version. This signals to users that the update might break their existing implementations.

2. `MINOR Version Increment:` When adding new features or functionality in a backward-compatible manner, increment the MINOR version. This informs users that they can safely update to access new capabilities.

3. `PATCH Version Increment:` For backward-compatible bug fixes and patches, increment the PATCH version. Users can confidently update to resolve issues without worrying about breaking changes.

4. `Pre-release Versions:` When working on pre-release versions, use identifiers like -alpha, -beta, or -rc to indicate that the software is not yet considered stable. Users can opt to test these versions but should be cautious about using them in production.

5. `Build Metadata:` Build metadata, indicated by the + sign, is typically used for internal purposes, such as tracking builds or build configurations. It does not impact version precedence.

**Version Comparison:**

When comparing SemVer versions, follow these rules:

- Versions are compared from left to right, starting with MAJOR.

- When comparing MAJOR versions, higher numbers have greater precedence.

- For MINOR and PATCH versions, higher numbers have greater precedence.

- Pre-release versions have lower precedence than the associated normal version. For example, 1.2.3 is greater than 1.2.3-alpha.

**Best Practices for Using Semantic Versioning:**

1. `Start at 1.0.0:` Begin with 1.0.0 for your initial release. This signifies that your project has reached a stable state.

2. `Use ^ or ~ for Dependency Ranges:` When specifying dependencies in your project's package.json, use ^ (caret) or ~ (tilde) followed by a version to define a range. This allows for automatic updates while respecting SemVer rules.

- ^1.2.3 allows updates to 1.x.x versions.
- ~1.2.3 allows updates to 1.2.x versions.

3. `Follow SemVer Strictly:` Adhere to SemVer principles rigorously to ensure that version numbers convey accurate information about changes in your software.

4. `Document Changes:` Maintain a changelog or release notes to inform users about what's new, changed, or fixed in each version.

5. `Use Pre-release Versions Wisely:` Reserve pre-release versions for testing and experimentation. Clearly communicate their purpose to users.

6. `Backwards Compatibility:` Prioritize maintaining backward compatibility, especially in MAJOR version updates.

## File System and Streams

### Reading files using blocking mode

In Node.js, you can read files in both blocking and non-blocking (asynchronous) modes. When you read a file in blocking mode, the program waits for the file operation to complete before moving on to the next task. This approach is simple but can lead to performance issues in applications with high concurrency requirements.

To read a file synchronously in Node.js, you can use the built-in fs (file system) module. Specifically, you'll use the fs.readFileSync() method, which reads the entire contents of a file and returns them as a string or a buffer.

```js
const filePath = "example.txt";

try {
  const fileData = fs.readFileSync(filePath, "utf8");
  console.log("File contents:", fileData);
} catch (error) {
  console.error("Error reading the file:", error.message);
}
```

Output:

```bash +@output
Error reading the file: fs is not defined
```

Use the fs.readFileSync() method to read a file in blocking mode. This method takes two arguments: the file path and an optional encoding (default is 'utf8' for text files). For example, to read a text file named "example.txt,".

**When to Use Blocking File Reads:**

Blocking file reads can be appropriate in certain scenarios, such as:

- `Simple Scripts:` For small, one-time scripts where file reads are not a performance bottleneck.

- `Initialization:` During application initialization or setup processes, blocking reads can simplify the code and ensure that configuration files are fully loaded before proceeding.

- `Error Handling:` When immediate and synchronous error handling is required.

### Non blocking file operations: Read, Write and Both

In Node.js, non-blocking file operations are essential for building efficient and responsive applications, especially in scenarios with high concurrency. These operations include reading, writing, and reading & writing files asynchronously.

**1. Reading Files Asynchronously:**

To read a file asynchronously in Node.js, you can use the fs.readFile() method. This method takes the file path and a callback function as arguments. Here's an example:

```js
const fs = require("fs");

const filePath = "example.txt";

fs.readFile(filePath, "utf8", (err, data) => {
  if (err) {
    console.error("Error reading the file:", err.message);
    return;
  }
  console.log("File contents:", data);
});
```

In this example, the file is read asynchronously, and the callback function is executed when the operation is complete.

**2. Writing Files Asynchronously:**

To write to a file asynchronously in Node.js, you can use the fs.writeFile() method. This method takes the file path, data to write, and a callback function. Here's an example:

```js
const fs = require("fs");

const filePath = "output.txt";
const fileData = "This is some data to write to the file.";

fs.writeFile(filePath, fileData, "utf8", (err) => {
  if (err) {
    console.error("Error writing to the file:", err.message);
    return;
  }
  console.log("File written successfully.");
});
```

Output:

```bash +@output
File written successfully.
```

In this example, we asynchronously write data to a file, and the callback function is executed when the operation is complete.

**3. Reading and Writing Files Asynchronously:**

You can also read a file, process its content, and then write to another file asynchronously using a combination of fs.readFile() and fs.writeFile() methods. Here's an example:

```js
const fs = require("fs");

const inputFilePath = "input.txt";
const outputFilePath = "output.txt";

fs.readFile(inputFilePath, "utf8", (err, data) => {
  if (err) {
    console.error("Error reading the input file:", err.message);
    return;
  }

  // Process data here, e.g., transform it

  fs.writeFile(outputFilePath, processedData, "utf8", (err) => {
    if (err) {
      console.error("Error writing to the output file:", err.message);
      return;
    }
    console.log("File written successfully.");
  });
});
```

This example reads data from one file, processes it, and then writes the processed data to another file asynchronously.

### Streams

Streams in Node.js provide a powerful way to work with data, allowing you to process large amounts of information efficiently and in a non-blocking manner.

**Difference Between Streaming and Non-Streaming Mode:**

Non-Streaming Mode:

In a non-streaming mode, data is typically loaded into memory entirely before any processing can occur. For example, if you read a large file non-streamingly, you would load the entire file into memory and then work with its contents.

```js
const fs = require("fs");

// Non-streaming mode (loading entire file into memory)
fs.readFile("large-file.txt", "utf8", (err, data) => {
  if (err) {
    console.error(err);
    return;
  }
  // Process data here
  console.log(data);
});
```

Output:

```bash +@output
{
  errno: -4058,
  code: 'ENOENT',
  syscall: 'open',
  path: 'C:\\Users\\PC2\\Desktop\\Projects\\Training\\large-file.txt'
}
```

Streaming Mode:

In a streaming mode, data is processed in smaller chunks as it becomes available. Instead of reading the entire data into memory at once, you work with pieces of data as they are streamed. This approach is memory-efficient and well-suited for processing large files or handling real-time data.

```js
const fs = require("fs");

// Streaming mode (processing data in chunks)
const stream = fs.createReadStream("large-file.txt", "utf8");

stream.on("data", (chunk) => {
  // Process the chunk of data
  console.log(chunk);
});

stream.on("end", () => {
  // All data has been processed
  console.log("Stream ended");
});
```

**Back Pressure:**

Back pressure is an important concept in streaming. It refers to the mechanism by which a slower consumer can signal a faster producer to slow down the rate of data transfer. Without back pressure, a fast producer could overwhelm a slow consumer, potentially leading to memory exhaustion or application crashes

Node.js provides built-in back-pressure mechanisms in its streams, which help maintain a balance between producers and consumers. Here's how it works:

```js
const fs = require("fs");

const readStream = fs.createReadStream("large-file.txt");
const writeStream = fs.createWriteStream("output.txt");

readStream.on("data", (chunk) => {
  // Simulate a slower consumer
  setTimeout(() => {
    // Write the chunk to the output stream
    writeStream.write(chunk);
  }, 100);
});

writeStream.on("drain", () => {
  // The write stream is ready to receive more data
  console.log("Back pressure relieved");
});

readStream.on("end", () => {
  // All data has been read
  writeStream.end();
});
```

In this example, if the write stream becomes overwhelmed, it emits a 'drain' event when it's ready to accept more data. This event allows the producer (read stream) to slow down its data production until the consumer is ready to handle more.

## Http Module

### What is HTTP

The Hypertext Transfer Protocol (HTTP) is a fundamental protocol of the World Wide Web (WWW). It defines the structure of requests and responses that are exchanged between a client (typically a web browser) and a server. HTTP is an application layer protocol that forms the basis of data communication on the internet.

**Key Features of HTTP:**

1. `Stateless Protocol:` HTTP is a stateless protocol, which means that each request-response pair is independent and does not store any information about previous requests. This makes it simple and scalable but also necessitates mechanisms like cookies for maintaining state between requests.

2. `Text-Based:` HTTP messages are text-based, making them human-readable and easy to debug. They consist of a request or response line followed by headers and, optionally, a message body.

3. `Connectionless:` Each HTTP request/response cycle operates independently of others, and the connection is closed after the response is sent. However, keep-alive mechanisms (HTTP/1.1 and later) allow multiple requests and responses to share the same connection, reducing latency.

4. `Protocol for the Web:` HTTP was designed for the web, where it enables the retrieval and display of hypertext documents. It has since been extended to support various media types, including images, videos, and application data.

**HTTP Methods:**

HTTP defines several request methods or verbs, each indicating the desired action to be performed on a resource. The most commonly used methods include:

- `GET:` Retrieve data from the server. It is idempotent, meaning multiple identical requests should have the same effect as a single request.

- `POST:` Submit data to be processed by the identified resource. It is not idempotent, as multiple identical requests may have different effects.

- `PUT:` Update a resource or create it if it doesn't exist. It is idempotent.

- `DELETE:` Remove the specified resource. It is idempotent.

- `HEAD:` Retrieve the headers of a resource without the actual content. It is used for checking resource metadata.

- `OPTIONS:` Retrieve information about the communication options for the target resource.

- `PATCH:` Apply partial modifications to a resource.

**HTTP Headers:**

HTTP headers are key-value pairs that provide additional information about the request or response. Some common headers include:

- `Host:` Specifies the domain name of the server (mandatory in HTTP/1.1).

- `User-Agent:` Identifies the user agent making the request (e.g., the web browser).

- `Content-Type:` Describes the media type of the resource in the message body.

- `Content-Length:` Indicates the size of the message body in octets (bytes).

- `Accept:` In a request, specifies the media types that the client can process. In a response, indicates the media type that the server selected.

- `Location:` In a response, specifies a different URI where the client can find the resource.

- `Set-Cookie:` Sets a cookie on the client's browser for maintaining state.

- `Authorization:` Contains credentials for authenticating the client to the server.

**HTTP Versions:**

HTTP has undergone several major revisions:

- `HTTP/0.9:` The earliest version, used to transfer hypertext documents.

- `HTTP/1.0:` Introduced features like request headers and response status codes. However, it relied on opening a new connection for each request.

- `HTTP/1.1:` Improved performance by introducing persistent connections (keep-alive), pipelining, and caching. It is still widely used today.

- `HTTP/2:` Introduced multiplexing, allowing multiple requests and responses to be sent in parallel over a single connection. It also provides header compression to reduce overhead.

- `HTTP/3:` Based on the QUIC transport protocol, HTTP/3 aims to further improve performance and security. It is designed to reduce latency and improve connection resilience.

**Security and HTTPS:**

HTTP is inherently unsecured, as data is transmitted in plaintext. To address this issue, the Hypertext Transfer Protocol Secure (HTTPS) was introduced. HTTPS uses encryption (typically TLS/SSL) to secure the communication between the client and server, ensuring data confidentiality and integrity. It has become the standard for secure web communication.

### REST Api

A Representational State Transfer (REST) API is a widely adopted architectural style for designing networked applications. RESTful APIs are known for their simplicity, scalability, and ability to leverage existing web technologies.

**Key Concepts of RESTful APIs:**

1. `Resources:`

- Central to REST is the concept of resources, which are the key abstractions. Resources can represent entities such as users, products, or articles.
- Resources are identified by Uniform Resource Identifiers (URIs) or URLs. Each resource has a unique URI.
- Resources can have multiple representations, such as JSON or XML, to support different data formats.

2. `HTTP Methods:`

- RESTful APIs use HTTP methods (also known as verbs) to define actions on resources.
- Common HTTP methods include:
  - GET: Retrieve resource data.
  - POST: Create a new resource.
  - PUT: Update an existing resource (or create if it doesn't exist).
  - DELETE: Remove a resource.
- HTTP methods are idempotent, meaning that repeated requests have the same effect as a single request (except for POST).

3. `Statelessness:`

- REST APIs are stateless, meaning that each request from a client to a server must contain all the information needed to understand and process the request.
- No session state is stored on the server between requests. Session state, if needed, should be managed on the client side.

4. `Representations:`

- Resources can have multiple representations, such as JSON, XML, or HTML.
- Clients can request specific representations by specifying the desired media type in the request headers (e.g., Accept: application/json).

**Characteristics of RESTful APIs:**

1. `Uniform Interface:`

- A RESTful API should have a uniform and consistent interface, which simplifies client and server interactions.
- It follows a small set of well-defined conventions, such as standard HTTP methods and status codes.

2. `Statelessness:`

- Each request from a client to a server must contain all the information needed to understand and process the request.
- This allows for easy scalability and load balancing since each request can be treated independently.

3. `Resource-Based:`

- Resources are the central abstractions in RESTful APIs, and they are represented by URIs.
- Resources are manipulated using standard HTTP methods.

4. `Representation:`

- Resources can have multiple representations (e.g., JSON, XML) to support different client needs.
- The client can specify the desired representation using the Accept header.

5. `Self-Descriptive Messages:`

- Responses from the server should include metadata (e.g., links to related resources) to help clients navigate the API.

6. `Stateless Communication:`

- Each request from a client to a server must contain all the necessary information. The server should not store client state between requests.

**Status Codes:**

HTTP status codes are used to indicate the outcome of a request. Common status codes in RESTful APIs include:

- `200 OK:` Successful request.
- `201 Created:` Resource successfully created.
- `204 No Content:` Successful request with no response body.
- `400 Bad Request:` Invalid request by the client.
- `401 Unauthorized:` Authentication required or failed.
- `403 Forbidden:` Authentication succeeded, but the client doesn't have permission.
- `404 Not Found:` Resource not found.
- `405 Method Not Allowed:` Requested HTTP method is not supported for the resource.
- `500 Internal Server Error:` Server error.

**Best Practices:**

1. `Use Plural Nouns for Resource Names:` Use plural nouns (e.g., /users, /products) for resource endpoints to indicate collections.

2. `Versioning:` Include API versioning in the URI (e.g., /v1/users) to allow for backward compatibility as the API evolves.

3. `Use HTTP Status Codes Correctly:` Return appropriate HTTP status codes to convey the result of a request.

4. `Pagination:` Implement pagination for resource collections to handle large datasets efficiently (e.g., /users?page=2&limit=10).

5. `Authentication and Authorization:` Implement secure authentication and authorization mechanisms.

6. `Rate Limiting:` Consider implementing rate limiting to prevent abuse of the API.

7. `Documentation:` Provide comprehensive API documentation to help developers understand how to use your API.

8. `HATEOAS (Hypermedia as the Engine of Application State):` Optionally, use links in responses to allow clients to navigate the API dynamically.

### Creating a server

In Node.js, you can create a streaming HTTP server using the built-in http module. Streaming HTTP servers allow you to efficiently handle large volumes of data by using streams to send and receive data in chunks, making them ideal for building real-time or data-intensive web applications.

```js
const http = require("http");

const PORT = 3000;
const HOST = "localhost";

const server = http.createServer((req, res) => {
  // Set response headers
  res.setHeader("Content-Type", "text/plain");

  // Write data to the response stream
  res.write("Hello, ");
  res.write("World!");

  // End the response stream
  res.end();
});

server.listen(PORT, HOST, () => {
  console.log(`Server is running at http://${HOST}:${PORT}`);
});
```

Output:

```bash +@output
Server is running at http://localhost:3000
```

Import the http module. Create an HTTP server using the http.createServer() method. Specify the port and host to listen on, and start the server using the command `node index.js`( whichever the name of the file).

### How HTTP Module Uses Streams for API Requests:

The http module in Node.js uses streams internally to handle API requests and responses efficiently. When a client sends a request to your HTTP server, the server processes the request using streams. Here's a simplified overview of how it works:

1. `Request Stream:` When a client makes an API request (e.g., a GET request), the incoming data from the client is processed as a readable stream. This allows the server to read the request data in chunks, making it suitable for handling large request payloads.

2. `Response Stream:` When your server responds to the client, it uses a writable stream to send data back in chunks. This is especially useful for streaming data to the client as it becomes available, rather than waiting for the entire response to be generated.

3. `Efficiency:` Streams allow your server to efficiently process data without loading the entire request or response into memory at once. This is crucial for handling large files, streaming real-time data, or handling multiple concurrent requests.

Here's a simplified example of how the http module handles a request using streams:

```js
const http = require("http");

const server = http.createServer((req, res) => {
  // Incoming data from the client is a readable stream (req)
  req.on("data", (chunk) => {
    // Process the request data in chunks
    console.log("Received data chunk:", chunk.toString());
  });

  // Outgoing data to the client is a writable stream (res)
  // Sending a response in chunks
  res.write("Hello, ");
  res.write("World!");
  res.end();
});

server.listen(3000, () => {
  console.log("Server is running at http://localhost:3000");
});
```

Output:

```text +@output
Hello, World!
```

In this example, the server processes incoming request data in chunks and responds to the client using writable streams. This approach ensures that the server can handle large requests and efficiently stream data back to clients.

### Https Module

The https module in Node.js allows you to create secure HTTP servers and make secure client requests using the HTTPS protocol. It builds upon the functionality of the built-in http module while adding encryption and security features. HTTPS servers provide additional security by encrypting data that is being transmitted from a server to a client, plus it uses SSL/TLS certificates to verify the client. It is used widely on the internet, for secure communication over a network

HTTPS uses the TLS or Transport Layer Security encryption protocol, which was formerly known as Secure Sockets Layer or SSL. The encryption protocols of HTTPS give the ability to users on the web, to transfer or pass on sensitive information such as credit card numbers, banking information, login credentials, and more in a secure way.

**Advantages of HTTPS Over HTTP:**

HTTPS (Hypertext Transfer Protocol Secure) offers several advantages over HTTP:

1. `Data Encryption:` HTTPS encrypts the data transmitted between the client and server, making it difficult for attackers to intercept and read sensitive information.

2. `Data Integrity:` It ensures that the data remains unchanged during transmission. Any tampering with the data will result in an error.

3. `Authentication:` HTTPS provides authentication through digital certificates, verifying the identity of the server to the client, reducing the risk of man-in-the-middle attacks.

4. `SEO Benefits:` Search engines often favor HTTPS websites, resulting in improved search engine rankings

**Certificates**

There are two kinds certificates; those signed by a ‘Certified Author’, also known as CA, and those that are ‘Self-signed’.

A CA-signed certificate allows your users to trust the identity of your website and is recommended for the production environment. For testing or development purposes, a Self-signed certificate will do just fine.

Installing openssl

`Windows:`

1. Install Chocolatey from [here](https://chocolatey.org/install).
1. Open powershell with admin access.
1. Run ` Set-ExecutionPolicy AllSigned` command.
1. Run `Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))` to install Chocolatey package manager.
1. Run `choco` to verify the installation
1. Run `choco install openssl` to install openssl cli tool.
1. Open a new powersheel instance and Run `openssl version` to verify the installation.

`Mac:`

1. Run `brew uninstall openssl` to install openssl.

`Linux`

1. Run `sudo apt install openssl` to install openssl.

Generating self signed certificate

```bash
openssl req -x509 -sha256 -nodes -days 365 -newkey rsa:2048 -keyout privateKey.key -out certificate.crt
```

This command generates a self-signed certificate (certificate.crt) and a private key (privateKey.key) valid for 365 days. You can use these files for your local HTTPS server.

**Creating a https server**

```js
const https = require("https");
const fs = require("fs");

// Load the certificate and private key
const privateKey = fs.readFileSync("privateKey.key", "utf8");
const certificate = fs.readFileSync("certificate.crt", "utf8");

const credentials = { key: privateKey, cert: certificate };

const server = https.createServer(credentials, (req, res) => {
  res.writeHead(200, { "Content-Type": "text/plain" });
  res.end("Secure Hello, World!\n");
});

server.listen(443, () => {
  console.log("HTTPS Server is running on port 443");
});
```

In this example:

- We load the self-signed certificate and private key.
- We create an HTTPS server using https.createServer() and provide the certificate and private key as credentials.
- We define a request handler to respond with "Secure Hello, World!".
- The server listens on port 443, the default port for HTTPS.

If you use a self-signed certificate, your browser may display a security warning because the certificate is not trusted. To bypass this, you can add the certificate to your browser's trust store or use tools like Postman that allow you to accept self-signed certificates for testing purposes.

Make a call from postman to `https://localhost:443` to get the response `Secure Hello, World!`.

### Requesting data with http/https Module

**Making GET Requests:**

1. Import the required module (http for HTTP or https for HTTPS).

2. Specify the request options, including the host, path, and method.

3. Use the module's request() method to send the GET request.

4. Handle the response data using event listeners.

```js
const http = require("http");

const options = {
  hostname: "jsonplaceholder.typicode.com",
  path: "/posts/1",
  method: "GET",
};

const req = http.request(options, (res) => {
  let data = "";

  res.on("data", (chunk) => {
    data += chunk;
  });

  res.on("end", () => {
    console.log("GET Response:", JSON.parse(data));
  });
});

req.on("error", (error) => {
  console.error("Request error:", error);
});

req.end();
```

To make a GET request using the https module, simply replace http with https in the code above.

**Making POST Requests:**

1. Import the required module (http for HTTP or https for HTTPS).

2. Specify the request options, including the host, path, method (POST), headers, and the data to be sent in the request body.

3. Use the module's request() method to send the POST request.

4. Handle the response data using event listeners.

```js
const https = require("https");

const options = {
  hostname: "jsonplaceholder.typicode.com",
  path: "/posts",
  method: "POST",
  headers: {
    "Content-Type": "application/json",
  },
};

const postData = JSON.stringify({
  title: "Sample Post",
  body: "This is a sample post request.",
  userId: 1,
});

const req = https.request(options, (res) => {
  let data = "";

  res.on("data", (chunk) => {
    data += chunk;
  });

  res.on("end", () => {
    console.log("POST Response:", JSON.parse(data));
  });
});

req.on("error", (error) => {
  console.error("Request error:", error);
});

req.write(postData);
req.end();
```

In this example, we send a POST request with JSON data. Adjust the postData variable to contain the data you want to send in your request.

### Working with Routes

Routes are the endpoints in api. For example `/users`, `/home`, `/about`, `/login` etc. You can define routes and whenever a request is made to a particular endpoint, you can program the server to return a particular response.

```js
const http = require("http");

const server = http.createServer((req, res) => {
  if (req.url === "/") {
    // Handle the root route (e.g., display a homepage)
    res.writeHead(200, { "Content-Type": "text/plain" });
    res.end("Welcome to the homepage!");
  } else if (req.url === "/about") {
    // Handle the "/about" route (e.g., display an about page)
    res.writeHead(200, { "Content-Type": "text/plain" });
    res.end("About us: We are an awesome company!");
  } else {
    // Handle 404 - Not Found for all other routes
    res.writeHead(404, { "Content-Type": "text/plain" });
    res.end("404 - Not Found");
  }
});

server.listen(3000, () => {
  console.log("Server is running on port 3000");
});
```

Output:

```text +@output
Welcome to the homepage!
```

Start the server and make request to `localhost:3000/` to get `Welcome to the homepage!` response. This is how you define a route and handle the response.

### Parsing URLs and Query Strings

In Node.js, you can parse URLs and query strings using the built-in http module and the url module. Parsing URLs is essential when working with web applications, as it allows you to extract information from the request URL and query parameters.

We can use query string to send data to the server. We can return the appropriate data back to client based on the request data.

**Parsing URLs and Query string with the url Module:**

The url module in Node.js provides utilities for URL resolution and parsing. You can use it to parse URLs from incoming HTTP requests. Here's how to do it:

```js
const http = require("http");
const url = require("url");

const server = http.createServer((req, res) => {
  // Parse the request URL
  const parsedUrl = url.parse(req.url, true);

  // Extract information from the parsed URL
  const pathname = parsedUrl.pathname; // URL path
  const query = parsedUrl.query; // Query parameters as an object

  res.writeHead(200, { "Content-Type": "text/plain" });

  // Respond with parsed information
  res.end(`Path: ${pathname}\nQuery: ${JSON.stringify(query)}`);
});

server.listen(3000, () => {
  console.log("Server is running on port 3000");
});
```

In this example:

1. We import the url module along with the http module.
2. Inside the request handler, we parse the request URL using url.parse().
3. We pass the req.url and true as arguments to url.parse() to also parse the query string into an object.
4. We extract the URL path and query parameters from the parsed URL and respond with them.

From the browser call the url `localhost:3000/getUser??name=John&age=30`

Output:

```text +@output
Path: /some/path
Query: {"name":"John","age":"30"}
```

### CURD app

Lets building a CURD (Create, Update, Read, Delete) application for a resource todos. We will use a json file to store our todos. Lets create REST api to interact with todos.

```json data.json
{
  "todos": [
    { "id": 1, "task": "Buy groceries", "completed": false },
    { "id": 2, "task": "Walk the dog", "completed": true }
  ]
}
```

```js index.js
const http = require("http");
const fs = require("fs");

const PORT = 3000;
const dataFilePath = "./data.json";

const server = http.createServer((req, res) => {
  if (req.method === "GET" && req.url === "/todos") {
    // Read todos from data.json and send as JSON response
    fs.readFile(dataFilePath, "utf-8", (err, data) => {
      if (err) {
        res.writeHead(500, { "Content-Type": "application/json" });
        res.end(JSON.stringify({ error: "Internal Server Error" }));
        return;
      }

      const todos = JSON.parse(data).todos;
      res.writeHead(200, { "Content-Type": "application/json" });
      res.end(JSON.stringify(todos));
    });
  } else if (req.method === "POST" && req.url === "/todos") {
    // Create a new todo
    let requestBody = "";
    req.on("data", (chunk) => {
      requestBody += chunk.toString();
    });
    req.on("end", () => {
      const newTodo = JSON.parse(requestBody);
      fs.readFile(dataFilePath, "utf-8", (err, data) => {
        if (err) {
          res.writeHead(500, { "Content-Type": "application/json" });
          res.end(JSON.stringify({ error: "Internal Server Error" }));
          return;
        }

        const todos = JSON.parse(data).todos;
        const id = todos.length + 1;
        newTodo.id = id;
        todos.push(newTodo);

        fs.writeFile(dataFilePath, JSON.stringify({ todos }), (err) => {
          if (err) {
            res.writeHead(500, { "Content-Type": "application/json" });
            res.end(JSON.stringify({ error: "Internal Server Error" }));
            return;
          }

          res.writeHead(201, { "Content-Type": "application/json" });
          res.end(JSON.stringify(newTodo));
        });
      });
    });
  } else if (req.method === "PUT" && req.url.startsWith("/todos/")) {
    // Update a todo by ID
    const todoId = parseInt(req.url.split("/")[2]);

    let requestBody = "";
    req.on("data", (chunk) => {
      requestBody += chunk.toString();
    });
    req.on("end", () => {
      const updatedTodo = JSON.parse(requestBody);

      fs.readFile(dataFilePath, "utf-8", (err, data) => {
        if (err) {
          res.writeHead(500, { "Content-Type": "application/json" });
          res.end(JSON.stringify({ error: "Internal Server Error" }));
          return;
        }

        const todos = JSON.parse(data).todos;
        const existingTodo = todos.find((todo) => todo.id === todoId);

        if (!existingTodo) {
          res.writeHead(404, { "Content-Type": "application/json" });
          res.end(JSON.stringify({ error: "Todo not found" }));
          return;
        }

        Object.assign(existingTodo, updatedTodo);

        fs.writeFile(dataFilePath, JSON.stringify({ todos }), (err) => {
          if (err) {
            res.writeHead(500, { "Content-Type": "application/json" });
            res.end(JSON.stringify({ error: "Internal Server Error" }));
            return;
          }

          res.writeHead(200, { "Content-Type": "application/json" });
          res.end(JSON.stringify(existingTodo));
        });
      });
    });
  } else if (req.method === "DELETE" && req.url.startsWith("/todos/")) {
    // Delete a todo by ID
    const todoId = parseInt(req.url.split("/")[2]);

    fs.readFile(dataFilePath, "utf-8", (err, data) => {
      if (err) {
        res.writeHead(500, { "Content-Type": "application/json" });
        res.end(JSON.stringify({ error: "Internal Server Error" }));
        return;
      }

      const todos = JSON.parse(data).todos;
      const indexToDelete = todos.findIndex((todo) => todo.id === todoId);

      if (indexToDelete === -1) {
        res.writeHead(404, { "Content-Type": "application/json" });
        res.end(JSON.stringify({ error: "Todo not found" }));
        return;
      }

      const deletedTodo = todos.splice(indexToDelete, 1)[0];

      fs.writeFile(dataFilePath, JSON.stringify({ todos }), (err) => {
        if (err) {
          res.writeHead(500, { "Content-Type": "application/json" });
          res.end(JSON.stringify({ error: "Internal Server Error" }));
          return;
        }

        res.writeHead(200, { "Content-Type": "application/json" });
        res.end(JSON.stringify(deletedTodo));
      });
    });
  } else {
    // Handle other routes or methods
    res.writeHead(404, { "Content-Type": "application/json" });
    res.end(JSON.stringify({ error: "Not Found" }));
  }
});

server.listen(PORT, () => {
  console.log(`Server is running on port ${PORT}`);
});
```

We check the type of call using `req.method`. Based on that we perform CURD operation on todos. We use `fs` module to read and write data to `data.json` file. This way implementation is hard to read and maintain. Node.js ecosystem has many packages that simplifies this process and provides tons of features. One such package is `express.js`. Lets explore more in the next section.

## Express.js

### What is Express js & Why Express js

Express.js, often referred to as Express, is a widely used and highly popular web application framework for Node.js. It simplifies the process of building scalable and robust web applications by providing a range of powerful features and tools.

Express.js is a minimal and flexible Node.js web application framework designed for building web applications and APIs. It is built on top of the core HTTP module in Node.js, which means it leverages the low-level capabilities of Node.js while providing a more structured and feature-rich environment for developing web applications.

**Key characteristics and features of Express.js include:**

1. `Middleware:` Express.js is known for its middleware architecture. Middleware functions can be thought of as a chain of functions that process incoming HTTP requests before they reach the application's routes. Middleware can perform tasks like authentication, logging, data parsing, and more.

2. `Routing:` Express provides a simple and powerful routing system that allows developers to define routes based on HTTP methods and URL patterns. This makes it easy to create RESTful APIs and define routes for handling various HTTP requests.

3. `Template Engines:` Although not bundled with Express itself, developers can easily integrate template engines like EJS, Handlebars, or Pug (formerly known as Jade) to generate dynamic HTML content. This is useful for rendering views on the server side.

4. `HTTP Utility Methods:` Express simplifies working with HTTP methods and status codes. It provides methods for common HTTP operations like GET, POST, PUT, DELETE, and more. This helps in writing concise and readable code.

5. `Error Handling:` Express includes error handling mechanisms to gracefully handle errors that may occur during the request-response cycle. This ensures that applications remain stable and provide meaningful error messages.

6. `Session Management:` Although not included in the core package, Express can be extended with middleware like express-session to manage user sessions and handle session-based authentication.

7. `Static File Serving:` Express can serve static files such as CSS, JavaScript, and images with ease, making it suitable for both API development and serving client-side applications.

**Why Express.js?**

Developers choose Express.js for various reasons, making it one of the most popular choices for building web applications and APIs:

1. `Simplicity:` Express.js follows a minimalistic and unopinionated approach, allowing developers to choose the libraries and tools they prefer. It provides essential features while giving developers the freedom to structure their applications as they see fit.

2. `Middleware Ecosystem:` Express's middleware ecosystem is extensive, offering a wide range of pre-built middleware packages that simplify common tasks. Developers can also create custom middleware to suit their specific needs.

3. `Community and Documentation:` Express has a large and active community, which means there are numerous resources, tutorials, and libraries available to assist developers. The official documentation is comprehensive and well-maintained.

4. `Flexibility:` Express.js can be used to build a variety of web applications, including APIs, single-page applications (SPAs), and traditional server-rendered web applications. Its flexibility allows it to adapt to different project requirements.

5. `Performance:` Express.js is known for its high performance and low overhead. It is designed to handle a large number of concurrent connections efficiently, making it suitable for high-traffic applications.

6. `Compatibility:` Express can be used in conjunction with other Node.js libraries and frameworks. This allows developers to integrate additional functionality seamlessly.

7. `Scalability:` Express.js provides a foundation for building scalable applications. It doesn't impose rigid application structures, giving developers the freedom to design their applications to scale as needed.

8. `Mature and Stable:` Express has been around for years and has a proven track record in the industry. Many well-known companies and projects use Express for their web applications.

### Setting up express app

1. Initialize a Node.js project:

```bash
mkdir my-express-app
cd my-express-app
npm init -y
```

Creates a folder by name `my-express-app`. `npm init -y` creates `package.json` file and instantiates a project.

2. Install Express:

```bash
npm install express
```

3. Create an `index.js` file.

```js
const express = require("express");
const app = express(); // application object

// Define a route
app.get("/", (req, res) => {
  res.send("Hello, Express!");
});

// Start the server
const PORT = process.env.PORT || 3000;
app.listen(PORT, () => {
  console.log(`Server is running on port ${PORT}`);
});
```

The app object in Express.js is an instance of the Express application. It provides methods to configure routes, handle HTTP requests and responses, set up middleware, and more.

Let's break down the key parts of the code:

1. `Import Express:` First, we import the Express module.

2. `Create an Express App:` We create an instance of the Express application and assign it to the app variable.

3. `Define a Route:` Using the app.get() method, we define a route for handling HTTP GET requests to the root path '/'. When a GET request is made to the root URL, the provided callback function is executed, sending the response 'Hello, Express!'.

4. `Start the Server:` We specify a port number (in this case, 3000) and use the app.listen() method to start the Express server. The server will listen on the specified port, and a message is logged to the console when the server starts.

**app Object Features:**

- `Middleware:` Express middleware functions can be added to the application using app.use(). Middleware functions can perform tasks like authentication, logging, and data parsing. Here's an example of using middleware for logging:

```js
// Middleware for logging requests
app.use((req, res, next) => {
  console.log(`Received ${req.method} request at ${req.url}`);
  next(); // Continue processing
});
```

- `Route Parameters:` You can define routes with parameters using colons (:) in the route path. For example:

```js
app.get("/users/:userId", (req, res) => {
  const userId = req.params.userId;
  // Use the userId in your logic
});
```

- `Static Files:` You can serve static files (e.g., CSS, JavaScript, images) using express.static middleware:

```js
app.use(express.static("public")); // Serve static files from the 'public' directory
```

- `Error Handling:` Express has built-in error handling using middleware. You can define error-handling middleware functions that take four parameters (err, req, res, next):

```js
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(500).send("Something broke!");
});
```

- `Additional HTTP Methods:` Besides app.get(), you can use methods like app.post(), app.put(), app.delete(), etc., to handle other HTTP methods. You dont have to check for request method type using `req.method` within an if condition.

```js
const express = require("express");
const app = express();

app.get("/users", (req, res) => {}); // gets all users
app.post("/users", (req, res) => {}); // creates user
app.put("/users/:userId", (req, res) => {}); // updates a user using userId
app.delete("/users/:userId", (req, res) => {}); // deletes a user using userId
```

- `Route Separation:` You can organize your routes in separate modules and use them with app.use() to create a modular Express application.

```js
const userRoutes = require("./userRoutes");

app.use(userRoutes); // userRoutes is a module with routes defined using express router
```

### Routes and Modularization

Lets see how to define routes in express. Lets create a todos example.

**Basic CRUD API for "todos"**

```js index.js
const express = require("express");
const app = express();
const PORT = 3000;

// Sample data - stored in a local variable (for simplicity)
let todos = [
  { id: 1, task: "Buy groceries", completed: false },
  { id: 2, task: "Walk the dog", completed: true },
  // Add more todos here
];

app.use(express.json());

// Get all todos
app.get("/todos", (req, res) => {
  res.json(todos);
});

// Get a todo by ID
app.get("/todos/:id", (req, res) => {
  const id = parseInt(req.params.id);
  const todo = todos.find((t) => t.id === id);
  if (!todo) return res.status(404).json({ error: "Todo not found" });
  res.json(todo);
});

// Create a new todo
app.post("/todos", (req, res) => {
  const newTodo = req.body;
  newTodo.id = todos.length + 1;
  todos.push(newTodo);
  res.status(201).json(newTodo);
});

// Update a todo by ID
app.put("/todos/:id", (req, res) => {
  const id = parseInt(req.params.id);
  const updatedTodo = req.body;
  const todoIndex = todos.findIndex((t) => t.id === id);
  if (todoIndex === -1)
    return res.status(404).json({ error: "Todo not found" });
  todos[todoIndex] = updatedTodo;
  res.json(updatedTodo);
});

// Delete a todo by ID
app.delete("/todos/:id", (req, res) => {
  const id = parseInt(req.params.id);
  const todoIndex = todos.findIndex((t) => t.id === id);
  if (todoIndex === -1)
    return res.status(404).json({ error: "Todo not found" });
  const deletedTodo = todos.splice(todoIndex, 1)[0];
  res.json(deletedTodo);
});

app.listen(PORT, () => {
  console.log(`Server is running on port ${PORT}`);
});
```

With core http module we have to add if else checks to check for method type and route. Express provides simple methods to do the same. We are storing the todos in a local variable. All the routes are refering that same variable. Adding all the roues within the index file is not manageable. Also in an actual application we will have more resources, complex business logic and Database connection. Lets see how modularization makes the code better.

**Benefits of Modularization:**

Modularization involves breaking down your Express application into separate modules or files, each handling specific functionality. It offers several advantages, including improved code organization, maintainability, and scalability. Here's how you can modularize the above code:

1. `Create a todos.js Module (todosRouter.js):`

```js index.js
const express = require("express");
const router = express.Router();

let todos = [
  { id: 1, task: "Buy groceries", completed: false },
  { id: 2, task: "Walk the dog", completed: true },
  // Add more todos here
];

// Get all todos
router.get("/", (req, res) => {
  res.json(todos);
});

// Get a todo by ID
router.get("/:id", (req, res) => {
  const id = parseInt(req.params.id);
  const todo = todos.find((t) => t.id === id);
  if (!todo) return res.status(404).json({ error: "Todo not found" });
  res.json(todo);
});

// Create a new todo
router.post("/", (req, res) => {
  const newTodo = req.body;
  newTodo.id = todos.length + 1;
  todos.push(newTodo);
  res.status(201).json(newTodo);
});

// Update a todo by ID
router.put("/:id", (req, res) => {
  const id = parseInt(req.params.id);
  const updatedTodo = req.body;
  const todoIndex = todos.findIndex((t) => t.id === id);
  if (todoIndex === -1)
    return res.status(404).json({ error: "Todo not found" });
  todos[todoIndex] = updatedTodo;
  res.json(updatedTodo);
});

// Delete a todo by ID
router.delete("/:id", (req, res) => {
  const id = parseInt(req.params.id);
  const todoIndex = todos.findIndex((t) => t.id === id);
  if (todoIndex === -1)
    return res.status(404).json({ error: "Todo not found" });
  const deletedTodo = todos.splice(todoIndex, 1)[0];
  res.json(deletedTodo);
});

module.exports = router;
```

Create a todoRouter.js file to add all the routes related to todos. Create a `router` instance of `express.Router()`. Instead of using REST methods on app object, we can use it on the router object. Finally export it and import it in the index file. Use `app.use()` method to add the todoRouter. `app.use('/todos', todoRouter);k` this line attaches the todoRouter to express app.

### Middlewares

Middleware plays a crucial role in Express.js, allowing you to add functionality to the request-response pipeline. Middleware is a series of functions that are executed in the order they are defined when an HTTP request is made to an Express.js application. These functions have access to the request (req) and response (res) objects and can perform various tasks, such as logging, data validation, authentication, and more.

**Types of Middleware:**

1. `Application-level Middleware:` These are middleware functions that are applied to the entire application. They are defined using app.use() and are executed for every incoming request.

2. `Router-level Middleware:` These are middleware functions applied to a specific router using router.use(). They only affect routes defined within that router.

3. `Error-handling Middleware:` These middleware functions handle errors. They have four parameters (err, req, res, next) and are defined with an extra parameter.

**Built-in Middlewares in Express.js:**

Express.js provides several built-in middleware functions to handle common tasks. Here are some of them:

1. `express.json():` Parses incoming JSON data from the request body.

```js
const express = require("express");
const app = express();

app.use(express.json());

app.post("/api/post", (req, res) => {
  console.log(req.body); // Access the JSON data
  res.json({ message: "Data received successfully" });
});

app.listen(3000, () => {
  console.log("Server is running on port 3000");
});
```

2. `express.urlencoded():` Parses incoming URL-encoded data (e.g., form submissions) from the request body.

```js
const express = require("express");
const app = express();

app.use(express.urlencoded({ extended: true }));

app.post("/api/form", (req, res) => {
  console.log(req.body); // Access URL-encoded data
  res.json({ message: "Form data received successfully" });
});

app.listen(3000, () => {
  console.log("Server is running on port 3000");
});
```

3. `express.static():` Serves static files (e.g., HTML, CSS, JavaScript, images) from a specified directory.

```js
const express = require("express");
const app = express();

app.use(express.static("public")); // Serve files from the 'public' directory

app.listen(3000, () => {
  console.log("Server is running on port 3000");
});
```

4. `Custom Middleware:` You can create custom middleware functions to perform specific tasks. Here's an example of a custom middleware that logs the request method and URL

```js
const express = require("express");
const app = express();

// Custom middleware
app.use((req, res, next) => {
  console.log(`Request Method: ${req.method}, URL: ${req.url}`);
  next(); // Call the next middleware
});

app.get("/", (req, res) => {
  res.send("Home Page");
});

app.get("/about", (req, res) => {
  res.send("About Page");
});

app.listen(3000, () => {
  console.log("Server is running on port 3000");
});
```

In this example, the custom middleware logs information about each incoming request before passing control to the next middleware or route handler.

### Serving static content

Static content are nothing but files which are served by server. For example html, css, js, images etc. Express has a middleware to do this. `express.static()` allows us to server all the content we want from a configured folder.

1. `Create a Directory for Your Static Files:`

Inside your project directory, create a folder to hold your static files. For example, you can create a public directory:

2. `Create Your HTML, CSS, and JavaScript Files:`

Place your HTML (index.html), CSS (styles.css), and JavaScript (script.js) files inside the public directory.

3. `Create your express server`

```js
const express = require("express");
const path = require("path");

const app = express();
const PORT = 3000;

app.use(express.static(path.join(__dirname, "public"))); // configs public folder as servable

// Define a route for the homepage
app.get("/", (req, res) => {
  res.send("Welcome to my static content app!");
});

app.listen(PORT, () => {
  console.log(`Server is running on port ${PORT}`);
});
```

```html index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Hello World Page</title>
    <link rel="stylesheet" href="../css/index.css" />
    <script src="../js/index.js"></script>
  </head>
  <body>
    <h1 onclick="showAlert()">Hello World</h1>
  </body>
</html>
```

```css index.css
body {
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background-color: lightblue;
}

h1 {
  cursor: pointer;
}

h1:hover {
  text-decoration: underline;
}
```

```js index.js
function showAlert() {
  alert("Hello World");
}
```

We pass the complete path of the `public` folder to the `express.static()` middleware. public folder has `index.html` file at its root. Now any request made to the server at `localhost:3000` will serve `index.html` file. Express takes care of the underlying logic for us. Within the html we import the css and js files. Both css and js files should be placed inside public folder for express to serve them. If not express will block the download of those files which browser attempts to.

When the `index.html` file is loaded by the browser. Browser also downloads all the css and js files linked within the html file. We can see the styles and event listeners added to the html element by css and js.

### MVC application

MVC (Model-View-Controller) is a design pattern commonly used in software development, including web applications. It separates an application into three interconnected components, each with a specific role:

1. `Model:` Represents the application's data and business logic. It interacts with the database (if applicable) and manages the application's state.

2. `View:` Represents the user interface (UI) and is responsible for displaying data to the user. It receives input from the user and forwards it to the controller for processing.

3. `Controller:` Acts as an intermediary between the model and the view. It receives user input from the view, processes it using the model, and updates the view with the results.

Instead of sending some text or json we send a html file. We make use of template engines to inject data into html and then serve the data populated html to the browser. We are going to use `ejs` as our template engine.

**Ejs Template engine**

EJS (Embedded JavaScript) is a popular template engine for Node.js and Express.js that allows you to generate dynamic HTML and other markup using JavaScript directly within your templates.

Features of EJS:

1. `JavaScript Integration:` EJS allows you to embed JavaScript code directly within your templates. This makes it easy to create dynamic content by executing JavaScript logic.

2. `Template Reusability:` EJS supports partials and layouts, enabling you to reuse templates and create modular views for your web application.

3. `Conditional Statements:` EJS provides conditional statements (<% if (condition) { %> ... <% } %>) for creating logic-based templates.

4. `Looping Constructs:` You can use JavaScript loops (<% for (let i = 0; i < data.length; i++) { %> ... <% } %>) to iterate over arrays and generate dynamic content.

5. Escaping:` EJS automatically escapes HTML entities to prevent cross-site scripting (XSS) attacks. You can use <%- ... %> to render unescaped HTML.

6. `Custom Functions:` EJS allows you to define custom JavaScript functions and use them within your templates for complex logic.

Basic Syntax:

- `<% ... %>:` Delimiters for embedding JavaScript code that doesn't produce any output.
- `<%= ... %>:` Delimiters for embedding JavaScript code that produces output (variables, expressions, etc.).
- `<%- ... %>:` Delimiters for embedding JavaScript code that produces unescaped output.

Usage in an Express.js Application:

- Configure EJS in Your Express App:

```js
const express = require("express");
const app = express();

app.set("view engine", "ejs");
app.set("views", __dirname + "/views");
```

- Create an EJS Template:

Create an EJS template file (e.g., template.ejs) in the views directory:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>EJS Template Example</title>
  </head>
  <body>
    <h1>Welcome to <%= pageTitle %></h1>
    <ul>
      <% for (let item of items) { %>
      <li><%= item %></li>
      <% } %>
    </ul>
  </body>
</html>
```

- Render the Template in an Express Route:

In your Express route handler, render the EJS template and pass data to it:

```js
app.get("/", (req, res) => {
  const data = {
    pageTitle: "EJS Example",
    items: ["Item 1", "Item 2", "Item 3"],
  };
  res.render("template", data);
});
```

Lets a build a todo application to handle CRUD operations from the browser using User interface.

1. Install the package `ejs` by running the command: `npm install ejs`.
2. Create a `views` folder to add all the html files. All the html files will have the extension of `.ejs`.
3. Create a `public` folder to add css files.

```js +index.js
const express = require("express");
const app = express();
const port = 3000;

// Middleware to parse JSON and URL-encoded data
app.use(express.json());
app.use(express.urlencoded({ extended: true }));

// Static files (CSS)
app.use(express.static("public"));

// In-memory data storage (for simplicity)
const todos = [];

// EJS Template Engine Setup
app.set("view engine", "ejs");
app.set("views", __dirname + "/views");

// Routes
app.get("/", (req, res) => {
  res.render("index", { todos });
});

app.post("/todos", (req, res) => {
  const newTodo = req.body.todo;
  todos.push(newTodo);
  res.redirect("/");
});

app.get("/todos/:id/edit", (req, res) => {
  const id = parseInt(req.params.id);
  const todo = todos[id];
  res.render("edit", { id, todo });
});

app.post("/todos/:id/edit", (req, res) => {
  const id = parseInt(req.params.id);
  const updatedTodo = req.body.todo;
  todos[id] = updatedTodo;
  res.redirect("/");
});

app.get("/todos/:id/delete", (req, res) => {
  const id = parseInt(req.params.id);
  todos.splice(id, 1);
  res.redirect("/");
});

app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});
```

We set the template engine that we are going to use and pass the reference to the folder where all our ejs files will be present.

```html -index.ejs
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>TODO App</title>
    <link rel="stylesheet" href="/css/index.css" />
  </head>
  <body>
    <div class="container">
      <h1>TODO App</h1>
      <form action="/todos" method="post">
        <input
          class="form-input"
          type="text"
          name="todo"
          placeholder="Add a new TODO"
          required
        />
        <button class="form-input" type="submit">Add</button>
      </form>
      <ul class="todo-list">
        <% todos.forEach((todo, index) => { %>
        <li>
          <%= todo %>
          <a href="/todos/<%= index %>/edit">Edit</a>
          <a href="/todos/<%= index %>/delete">Delete</a>
        </li>
        <% }); %>
      </ul>
    </div>
  </body>
</html>
```

```html -edit.ejs
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Edit TODO</title>
    <link rel="stylesheet" href="/css/index.css" />
  </head>
  <body>
    <div class="container">
      <h1>Edit TODO</h1>
      <form action="/todos/<%= id %>/edit" method="post">
        <input
          class="form-input"
          type="text"
          name="todo"
          value="<%= todo %>"
          required
        />
        <button class="form-input" type="submit">Save</button>
      </form>
    </div>
  </body>
</html>
```

```css -index.css
/* Add your styles here */
body {
  font-family: Arial, sans-serif;
  background-color: lightblue;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}

.container {
  text-align: center;
}

.form-input {
  padding: 10px;
  margin: 5px;
}

.todo-list {
  text-align: left;
  margin-top: 20px;
}

.todo-list li {
  list-style: none;
  margin-bottom: 10px;
}
```

## MongoDB

MongoDB is a document based NoSql database. document is the basic unit of mongodb. Documents don't need to have a particular schema. Group of documents is called a collection. This is what we would call a table in a NQl Database. Data is stored in the for BSON(Binary JSON) in database. This enables Mongodb to support more datatypes than JSON(Javascript Object Notation). MongoDB documents are not schema based. But we can add validation rules to specify the structure of a document.

### What is MongoDB

**SQL vs NoSQL**

SQL (Structured Query Language) and NoSQL (Not Only SQL) are two broad categories of database management systems, each with its own set of characteristics, advantages, and use cases.

SQL (Relational Databases):

1. `Data Structure:` SQL databases are relational, meaning they use structured tables to store data.
   Data in SQL databases is organized into rows and columns, forming tables with predefined schemas.

2. `Schema:` SQL databases have a fixed schema, meaning the structure of the database (e.g., table columns and data types) is defined before data is inserted.
   Schema changes can be complex and require careful management.

3. `Query Language:` SQL databases use the SQL query language for defining, manipulating, and querying data.
   SQL offers powerful querying capabilities with features like JOINs and transactions.

4. `ACID Transactions:` SQL databases generally support ACID (Atomicity, Consistency, Isolation, Durability) transactions, ensuring data integrity and consistency.

5. `Scalability:` SQL databases are traditionally scaled vertically (adding more resources to a single server).
   Scaling out (horizontal scaling) SQL databases can be challenging.

6. `Use Cases:` SQL databases are suitable for applications with structured and well-defined data, such as financial systems, e-commerce platforms, and applications requiring complex queries.

NoSQL (Non-Relational Databases):

1. `Data Structure:` NoSQL databases are non-relational and provide flexibility in data storage.
   Data can be stored in various formats, including JSON, XML, key-value pairs, and more.

2. `Schema:` NoSQL databases are schema-less or have a dynamic schema, allowing for easy adaptation to changing data requirements.
   Data can be added without a predefined structure.

3. `Query Language:` NoSQL databases use various query languages, often tailored to the specific database type (e.g., MongoDB uses BSON queries, Cassandra uses CQL).
   Query capabilities may vary between NoSQL databases.

4. `CAP Theorem:` NoSQL databases are often designed with the CAP theorem in mind, allowing for high availability and partition tolerance at the potential expense of consistency.
   Different NoSQL databases prioritize different aspects of the CAP theorem (e.g., some focus on consistency, while others prioritize availability).

5. `Scalability:` NoSQL databases are typically designed for horizontal scalability, making it easier to distribute data across multiple servers or nodes.
   They can handle large volumes of data and high traffic loads.

6. `Use Cases:` NoSQL databases are suitable for applications with evolving data structures, high scalability requirements, and real-time data processing needs. Use cases include social media platforms, IoT applications, and big data analytics.

The choice between SQL and NoSQL depends on the specific requirements of your application. Consider factors such as data structure, scalability needs, development speed, and the complexity of your queries when making your decision. Some projects even use a combination of both SQL and NoSQL databases to meet various data storage and retrieval needs.

### Document-oriented vs. other types of storage

"Document-oriented" is a specific type of data storage approach commonly associated with NoSQL databases, particularly in the context of databases like MongoDB. To understand "document-oriented" databases, it's helpful to compare them to other types of storage models commonly used in databases:

**1. Document-Oriented Databases:**

1. `Data Structure:` Document-oriented databases store data in documents, which are semi-structured or unstructured records often in formats like JSON or BSON (binary JSON). Each document can have different fields and structures.
2. `Schema Flexibility:` These databases offer flexible schemas, meaning you can add or remove fields in documents without affecting the entire dataset. This is ideal for scenarios where data is evolving or unpredictable.
3. `Complex Data:` They excel at handling complex, nested, or hierarchical data structures, making them suitable for applications dealing with diverse data types.
   Example: MongoDB is a popular document-oriented database.

**2. Relational Databases (SQL):**

1. `Data Structure:` Relational databases use tables to store data in rows and columns with a predefined schema. Data is structured and normalized to minimize redundancy.
2. `Schema Rigidity:` They have a rigid schema, where schema changes require careful planning and migrations. All rows in a table adhere to the same structure.
3. `Data Integrity:` Relational databases are designed for maintaining data integrity through features like foreign keys and referential constraints.
   Example: MySQL, PostgreSQL, Oracle Database.

**3. Key-Value Stores (NoSQL):**

1. `Data Structure:` Key-value stores store data as pairs of keys and associated values. Values can be simple strings or binary data.
2. `Schema Simplicity:` They are the simplest NoSQL databases with no complex data structures. Each key points to a single value.
3. `High Performance:` Key-value stores are known for their high performance and low latency, making them suitable for caching and real-time applications.
   Example: Redis, Amazon DynamoDB.

**4. Column-Family Stores (NoSQL):**

1. `Data Structure:` Column-family stores organize data into column families, which contain rows of data columns. Each row can have a different set of columns.
2. `Wide-Column Model:` They are designed for handling wide-column data, making them suitable for scenarios like time-series data or sparse data.
   Example: Apache Cassandra, HBase.

**5. Graph Databases (NoSQL):**

1. `Data Structure:` Graph databases represent data as nodes, edges, and properties. They excel at modeling and querying highly interconnected data.
2. `Relationships:` They are designed for efficiently querying relationships in data, making them ideal for social networks, recommendation engines, and network analysis.
   Example: Neo4j, Amazon Neptune.

Choosing the appropriate storage model depends on the specific requirements of your application. Document-oriented databases are favored when you need schema flexibility and handle semi-structured or hierarchical data. Other storage models, like relational, key-value, column-family, or graph databases, are better suited for different use cases based on their respective strengths and limitations.

### Features of MongoDB

MongoDB is a popular NoSQL database that offers a wide range of features and capabilities, making it suitable for various types of applications

1. `Flexible Schema:` MongoDB is schema-less or has a dynamic schema, allowing you to store and manage data without a predefined structure. This flexibility is particularly useful when dealing with evolving data.

2. `JSON-Like Documents:` MongoDB stores data in BSON (binary JSON) format, which is a JSON-like representation. Each data record is called a document, and documents can have different structures within the same collection.

3. `Highly Scalable:` MongoDB supports horizontal scaling, making it easy to distribute data across multiple servers or nodes. It can handle large volumes of data and high traffic loads.

4. `Automatic Sharding:` MongoDB provides built-in sharding capabilities for distributing data across multiple servers, ensuring data availability and horizontal scalability.

5. `Indexing:` MongoDB supports various types of indexes, including single-field, compound, geospatial, and text indexes. Indexing improves query performance.

6. `Ad Hoc Queries:` MongoDB supports ad hoc queries, allowing you to query data using a flexible and expressive query language. You can perform complex queries, including aggregation and text search.

7. `Replication:` MongoDB offers replica sets for data redundancy and high availability. Replica sets automatically elect a primary node and maintain secondary nodes for failover.

8. `Load Balancing:` MongoDB provides automated load balancing, distributing read operations across replica set members to improve query performance.

9. `Geospatial Queries:` MongoDB supports geospatial indexing and querying, making it suitable for location-based applications.

10. `Full-Text Search:` MongoDB includes a powerful full-text search engine, allowing you to perform text-based searches on documents.

11. `Aggregation Framework:` MongoDB's aggregation framework enables complex data transformations and analysis, including grouping, filtering, and data aggregation.

12. `Security:` MongoDB offers authentication, authorization, and role-based access control (RBAC) for securing data. It supports integration with LDAP and Kerberos.

13. `Data Encryption:` MongoDB provides encryption at rest and in transit to protect data privacy and security.

14. `Change Streams:` Change streams allow you to monitor real-time changes in the database, making it useful for building reactive applications.

15. `Cross-Platform Compatibility:` MongoDB is available on various platforms, including Linux, Windows, macOS, and cloud-based services.

16. `Rich Ecosystem:` MongoDB has a rich ecosystem of drivers, libraries, and tools for various programming languages and frameworks, making it easy to integrate with your tech stack.

17. `Community and Enterprise Editions:` MongoDB offers both a free community edition and a paid enterprise edition with additional features and support.

18. `Extensible:` MongoDB allows you to extend its functionality with custom JavaScript functions, triggers, and server-side scripts.

19. `Cloud Integration:` MongoDB Atlas, the official cloud-hosted MongoDB service, offers easy deployment and management of MongoDB databases in the cloud.

20. `Comprehensive Documentation:` MongoDB provides comprehensive documentation, tutorials, and educational resources for developers and administrators.

### Introduction to JSON

JSON (JavaScript Object Notation) is a lightweight and widely used data interchange format. It is easy for humans to read and write and easy for machines to parse and generate. JSON is often used to transmit data between a server and a web application, as well as between different parts of an application.

1. `Data Structure:` JSON represents data in a structured format consisting of key-value pairs. Each key is a string, followed by a colon, and then a value. The key-value pairs are separated by commas. JSON data is typically enclosed in curly braces {} to form an object or in square brackets [] to form an array.

Example of a JSON object:

```json
{
  "name": "John Doe",
  "age": 30,
  "city": "New York"
}
```

2. `Data Types:` JSON supports a limited set of data types:

- `Strings:` Enclosed in double quotes ("...").
- `Numbers:` Integer or floating-point numbers.
- `Boolean:` true or false.
- `Null:` Represents an empty value.
- `Object:` A collection of key-value pairs enclosed in curly braces.
- `Array:` An ordered list of values enclosed in square brackets.

3. `Nested Structures:` JSON allows nesting of objects and arrays within other objects or arrays, enabling the representation of complex and hierarchical data structures.

Example of a JSON object with nested structures:

```json
{
  "person": {
    "name": "Alice",
    "age": 25,
    "addresses": [
      { "type": "home", "city": "Boston" },
      { "type": "work", "city": "New York" }
    ]
  }
}
```

4. `Human-Readable:` JSON is designed to be easily readable by both humans and machines. The syntax is simple, with minimal punctuation.

5. `Language Agnostic:` JSON is not tied to any particular programming language and is supported by a wide range of programming languages. This makes it an ideal choice for data interchange between systems written in different languages.

6. `Use Cases:`

- `Web APIs:` JSON is commonly used for transmitting data between web servers and web clients in the form of HTTP responses.
- `Configuration Files:` JSON is used for configuration files in various applications and services.
- `Data Storage:` JSON is used as a data storage format for NoSQL databases like MongoDB.
- `Serialization:` JSON is used for serializing and deserializing data in web applications.

7. `JSON Schema:` JSON Schema is a specification for defining the structure, validation rules, and documentation for JSON data. It helps ensure that JSON data adheres to a predefined schema.

### Installing MongoDB

Download the mongodb for your operating system from [here](https://www.mongodb.com/docs/manual/installation/).

Download `mongosh` from [here](https://www.mongodb.com/docs/mongodb-shell/install/).
mongosh is a cli tool for interacting with mongodb.

Once the mongosh is installed run `mongosh` in the terminal. It opens up a shell to interact with local mongodb instance.

**Working with Databases**

```bash
// lists dbs
show dbs

// switches db
use todoapp

// deletes db
db.dropDatabase()
```

we switch to the db we want to delete using `use <somedb>`. Then run the command `db.dropDatabase()` to delete it.

`use` command switches the databse. Here `todoapp` was the db name so it switched to it. It doesn't create a db untill some data is added to it though.

### Documents and Collections

**Collections**

Collections are similar to tables in SQL.

```bash
// list collection
show collections

// create collection
db.createCollection("mycollection")

// delete collection
db.mycollection.drop()
```

**Documents**

```bash
// Create document
db.todos.insertOne({
  task: "Buy groceries",
  completed: false
})


// Create multiple documents
db.todos.insertMany([
  {
    task: "Finish project",
    completed: false
  },
  {
    task: "Exercise",
    completed: true
  }
])

// get all documents
db.todos.find()


// filter documents
db.todos.find({ completed: true })

// update documents
db.todos.updateOne(
  { task: "Buy groceries" },
  { $set: { completed: true } }
)

// update multiple documents
db.todos.updateMany(
  { completed: false },
  { $set: { completed: true } }
)

// delete documents
db.todos.deleteOne({ task: "Exercise" })


// delte multiple documents
db.todos.deleteMany({ completed: true })
```

### Simple Queries

**Sample data**

Todos

```js
[
  {
    task: "Complete project proposal",
    completed: false,
    priority: "High",
    tags: ["work", "project"],
    dueDate: "2023-09-15",
    category: "Business",
  },
  {
    task: "Buy groceries",
    completed: true,
    priority: "Medium",
    tags: ["personal", "shopping"],
    dueDate: "2023-09-10",
    category: "Personal",
  },
  {
    task: "Prepare for the presentation",
    completed: false,
    priority: "High",
    tags: ["work", "presentation"],
    dueDate: "2023-09-20",
    category: "Business",
  },
  {
    task: "Exercise for 30 minutes",
    completed: true,
    priority: "Low",
    tags: ["health", "exercise"],
    dueDate: "2023-09-12",
    category: "Personal",
  },
  {
    task: "Read a book",
    completed: false,
    priority: "Low",
    tags: ["personal", "reading"],
    dueDate: "2023-09-30",
    category: "Personal",
  },
];
```

products

```json
[
  {
    "name": "Laptop",
    "category": "Electronics",
    "price": 999.99,
    "in_stock": true
  },
  {
    "name": "Smartphone",
    "category": "Electronics",
    "price": 599.99,
    "in_stock": true,
    "brand": "Samsung",
    "model": "Galaxy S21",
    "color": "Phantom Black"
  },
  {
    "name": "The Great Gatsby",
    "category": "Books",
    "price": 14.99,
    "in_stock": true,
    "author": "F. Scott Fitzgerald",
    "genre": "Classic Fiction"
  },
  {
    "name": "Men's Jeans",
    "category": "Clothing",
    "price": 49.99,
    "in_stock": false,
    "brand": "Levi's",
    "size": "32W x 34L",
    "color": "Dark Blue"
  },
  {
    "name": "Coffee Maker",
    "category": "Appliances",
    "price": 79.99,
    "in_stock": true,
    "brand": "Keurig",
    "type": "Single Serve"
  }
]
```

User

```json
[
  {
    "name": "John Doe",
    "email": "john.doe@example.com",
    "age": 30,
    "password": "hashedpassword123",
    "address": {
      "city": "New York",
      "pincode": 10001
    }
  },
  {
    "name": "Alice Smith",
    "email": "alice.smith@example.com",
    "age": 28,
    "password": "hashedpassword456",
    "address": {
      "city": "Los Angeles",
      "pincode": 90001
    }
  },
  {
    "name": "Carlos Rodriguez",
    "email": "carlos.rodriguez@example.com",
    "age": 35,
    "password": "hashedpassword789",
    "address": {
      "city": "Madrid",
      "pincode": 28001
    }
  },
  {
    "name": "Emily Johnson",
    "email": "emily.johnson@example.com",
    "age": 25,
    "password": "hashedpasswordabc",
    "address": {
      "city": "Chicago",
      "pincode": 60601
    }
  },
  {
    "name": "Michael Brown",
    "email": "michael.brown@example.com",
    "age": 42,
    "password": "hashedpasswordxyz",
    "address": {
      "city": "San Francisco",
      "pincode": 94101
    }
  }
]
```

**Field Equality Tests:**

Field equality tests in MongoDB involve querying documents to find those that have a specific field equal to a specified value. These tests are commonly used to filter and retrieve documents that match a particular criterion based on one or more fields.

`Equality Operator: $eq`

The $eq operator is used to perform field equality tests. It matches documents where a specified field has a value that is equal to the specified value.

Example 1: Find todos with a specific task

```bash
db.todos.find({ task: "Buy groceries" })
```

Output

```mongosh +@output
> db.todos.find({task: "Buy groceries" })
[
  {
    _id: ObjectId("651e5f4df3b5b884192b8f70"),
    task: 'Buy groceries',
    completed: true,
    priority: 'Medium',
    tags: ['personal', 'shopping' ],
    dueDate: 2023-09-10'
    category: 'Personal'
  }
]
```

Example 2: Find users with a specific age

```bash
db.users.find({ age: 30 })
```

Output

```mongosh +@output
> db.users.find({age: 30})
[
  {
    _id: ObjectId("651e6260f3b5b884192b8f74"),
    name: 'John Doe',
    email: john.doe@example.com',
    age: 30,
    password: 'hashedpassword123',
    address: { city: 'New York', pincode: 10001 }
  }
]
```

`Multiple Equality Tests`

You can perform multiple field equality tests within the same query.

Example 3: Find users with a specific name and age

```bash
db.users.find({ name: "Alice", age: 25 })
```

`Using $eq with Arrays`

The $eq operator can also be used to match elements within arrays.

Example 4: Find todos with specific tags

```bash
db.todos.find({ tags: { $eq: ["grocery", "urgent"] } })
```

**Operators Available:**

In MongoDB, operators are special symbols or keywords used in queries to perform various operations on data fields. These operators allow you to filter, manipulate, and compare data in your queries. MongoDB provides a rich set of operators to query and manipulate data effectively.

`1. Equality Operators:` $eq: Matches values that are equal to a specified value.

Example: Find todos with a specific task.

```bash
db.todos.find({ task: "Buy groceries" })
```

Output

```mongosh +@output
> db.todos.find({task: "Buy groceries" })
[
  {
    _id: ObjectId("651e5f4df3b5b884192b8f70"),
    task: 'Buy groceries',
    completed: true,
    priority: 'Medium',
    tags: ['personal', 'shopping' ],
    dueDate: 2023-09-10'
    category: 'Personal'
  }
]
```

`2. Comparison Operators:`

- `$gt:` Matches values that are greater than a specified value.
- `$lt:` Matches values that are less than a specified value.
- `$gte:` Matches values that are greater than or equal to a specified value.
- `$lte:` Matches values that are less than or equal to a specified value.

Example: Find todos with a price greater than $10.

```bash
db.products.find({ price: { $gt: 10 } })
```

Output

```mongosh +@output
> db.products.find({ price: { $gt: 10 } })
[
  {
    _id: ObjectId("651e627df3b5b884192b8f79"),
    name: 'Laptop",
    category: 'Electronics',
    price: 999.99,
    in_stock: true
  },
  {
    _id: ObjectId("651e627df3b5b884192b8f7a"),
    name: 'Smartphone',
    category: Electronics',
    price: 599.99,
    in_stock: true,
    brand: Samsung',
    model: Galaxy S21',
    color: 'Phantom Black"
  },
  {
    _id: ObjectId("651e627df3b5b884192b8f7b"),
    name: 'The Great Gatsby',
    category: Books',
    price: 14.99,
    in_stock: true,
    author: 'F. Scott Fitzgerald',
    genre: 'Classic Fiction'
  },
  {
    _id: ObjectId("651e627df3b5b884192b8f7c"),
    name: "Men's Jeans",
    category: Clothing',
    price: 49.99,
    in_stock: false,
    brand: "Levi's",
    size: 32W x 34L',
    color: 'Dark Blue'
  },
  {
    _id: ObjectId("651e627df3b5b884192b8f7d"),
    name: 'Coffee Maker',
    category: 'Appliances',
    price: 79.99,
    in_stock: true,
    brand: Keurig',
    type: Single Serve'
  }
]
```

`3. Inequality Operators:`

- `$ne:` Matches values that are not equal to a specified value.
- `$nin:` Matches values that do not exist in a specified array.

Example: Find todos with a task not equal to "Exercise."

```bash
db.todos.find({ task: { $ne: "Exercise" } })
```

Output

```mongosh +@output
> db.todos.find({task: {$ne: "Exercise"}})
[
  { _id: ObjectId("651e5f4df3b5b884192b8f6f"),
    task: 'Complete project proposal',
    completed: false,
    priority: High",
    tags: ['work', 'project' ],
    dueDate: 2023-09-15',
    category: 'Business'
  },
  {
    _id: ObjectId("651e5f4df3b5b884192b8f70"),
    task: Buy groceries',
    completed: true,
    priority: 'Medium',
    tags: ['personal', 'shopping' ],
    dueDate: 2023-09-10',
    category: 'Personal'
  },
  {
    _id: ObjectId("651e5f4df3b5b884192b8f71"),
    task: 'Prepare for the presentation',
    completed: false,
    priority: High',
    tags: ['work', 'presentation' ],
    dueDate: 2023-09-20',
    category: 'Business'
  },
  {
    _id: ObjectId("651e5f4df3b5b884192b8f72"),
    task: 'Exercise for 30 minutes',
    completed: true,
    priority: Low,
    tags: ['health', 'exercise' ],
    dueDate: 2023-09-12",
    category: Personal'
  },
  {
    _id: ObjectId("651e5f4df3b5b884192b8f73"),
    task: 'Read a book',
    completed: false,
    priority: Low',
    tags: ['personal', 'reading' ],
    dueDate: 2023-09-30',
    category: 'Personal'
  }
]
```

`4. Logical Operators:`

- `$and:` Joins query clauses with a logical AND and returns documents that match all the conditions.
- `$or:` Joins query clauses with a logical OR and returns documents that match at least one of the conditions.
- `$not:` Inverts the effect of a query expression and returns documents that do not match the specified condition.

Example: Find todos that are either completed or have a priority of "High."

```bash
db.todos.find({ $or: [{ completed: true }, { priority: "High" }] })
```

Output

```mongosh +@output
> db.todos.find({$or: [{completed: true}, {priority: "High"}]})
[
  {
    _id: ObjectId("651e5f4df3b5b884192b8f6f"),
    task: 'Complete project proposal',
    completed: false,
    priority: 'High',
    tags: ['work', 'project'],
    dueDate: 2023-09-15',
    category: 'Business'
  },
  {
    _id: ObjectId("651e5f4df3b5b884192b8f70"),
    task: 'Buy groceries',
    completed: true,
    priority: Medium',
    tags: ['personal', 'shopping'],
    dueDate: 2023-09-10',
    category: Personal'
  },
  {
    _id: ObjectId("651e5f4df3b5b884192b8f71"),
    task: 'Prepare for the presentation',
    completed: false,
    priority: High',
    tags: ['work', 'presentation'],
    dueDate: 2023-09-20,
    category: 'Business'
  },
  {
    _id: ObjectId("651e5f4df3b5b884192b8f72"),
    task: Exercise for 30 minutes',
    completed: true,
    priority: 'Low",
    tags: [health', 'exercise'],
    dueDate: 2023-09-12',
    category: 'Personal'
  }
]
```

`5. Element Operators:`

- `$exists:` Matches documents where a specified field exists or does not exist.
- `$type:` Matches documents of a specific BSON data type.

Example: Find todos that have a due date field.

```bash
db.todos.find({ due_date: { $exists: true } })
```

`6. Array Operators:`

- `$in:` Matches any of the values in a specified array.
- `$nin:` Matches none of the values in a specified array.
- `$all:` Matches arrays that contain all elements specified in the query.

Example: Find todos in specific categories.

```bash
db.todos.find({ category: { $in: ["Work", "Personal"] } })
```

Output

```mongosh +@output
> db.todos.find({category: {$in: ["work", "Personal"]}})
[
  {
    _id: ObjectId("651e5f4df3b5b884192b8f70"),
    task: 'Buy groceries',
    completed: true,
    priority: Medium',
    tags: ['personal', 'shopping'],
    dueDate: 2023-09-10',
    category: Personal'
  },
  {
    _id: ObjectId("651e5f4df3b5b884192b8f72"),
    task: 'Exercise for 30 minutes',
    completed: true,
    priority: Low',
    tags: ['health', 'exercise' ],
    dueDate: 2023-09-12',
    category: Personal'
  },
  {
    _id: ObjectId("651e5f4df3b5b884192b8f73"),
    task: 'Read a book',
    completed: false,
    priority: Low',
    tags: ['personal', 'reading' ],
    dueDate: 2023-09-30',
    category: Personal'
  }
]
```

`7. Text Operators:`

- `$text:` Performs text search on a text index.

```bash
db.todos.find({ $text: { $search: "important" } })
```

`8. Array Update Operators:`

- `$push:` Adds an element to an array.
- `$pull:` Removes all instances of a value from an array.
- `$addToSet:` Adds an element to an array only if it doesn't already exist.

Example: Add a new task to a todo list.

```bash
db.todos.updateOne(
  { _id: ObjectId("todoId") },
  { $push: { tasks: "New task" } }
)
```

Output

```mongosh +@output
> db.todos.updateOne({_id: ObjectId("651e5f4df3b5b884192b8f70")}, {$push: {tasks: "New Task"}})
  {
    acknowledged: true,
    insertedId: null,
    matchedCount: 1,
    modifiedCount: 1,
    upsertedCount: 0
  }
```

**Projections:**

In MongoDB, "projections" refer to the ability to specify which fields should be included or excluded from the result set when querying documents from a collection. Projections allow you to shape the output of your queries by controlling the fields that are returned. This can be particularly useful for improving query performance, reducing network overhead, and ensuring that only the necessary data is retrieved.

`Including Fields in the Result:` To include specific fields in the result, you can use the { field: 1 } syntax in the projection argument of the find() method. The 1 indicates that the field should be included.

Example: Include only the "name" and "age" fields in the result:

```bash
db.users.find({}, { name: 1, age: 1 })
```

Output

```mongosh +@output
> db.users.find({}, {name:1, age: 1})
[
  {
    _id: ObjectId("651e6260f3b5b884192b8f74"), name: 'John Doe',
    age: 30
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f75"), name: 'Alice Smith',
    age: 28
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f76"), name: 'Carlos Rodriguez',
    age: 35
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f77"), name: 'Emily Johnson',
    age: 25
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f78"), name: 'Michael Brown',
    age: 42
  }
]
```

`Excluding Fields from the Result:` To exclude specific fields from the result, you can use the { field: 0 } syntax in the projection argument of the find() method. The 0 indicates that the field should be excluded.

```bash
db.users.find({}, { password: 0 })
```

Output

```mongosh +@output
> db.users.find({}, {password: 0})
[
  {
    _id: ObjectId("651e6260f3b5b884192b8f74"), name: John Doe',
    email: john.doe@example.com" ,
    age: 30,
    address: {city: 'New York', pincode: 10001 }
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f75"), name: Alice Smith',
    email: 'alice.smith@example.com',
    age: 28,
    address: { city: 'Los Angeles', pincode: 90001 }
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f76"), name: Carlos Rodriguez',
    email: 'carlos.rodriguez@example.com',
    age: 35,
    address: { city: 'Madrid', pincode: 28001 }
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f77"), name: 'Emily Johnson',
    email: emily.johnson@example.com',
    age: 25,
    address: {city: 'Chicago', pincode: 60601 }
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f78"), name: 'Michael Brown',
    email: 'michael.brown@example.com",
    age: 42,
    address: {city: 'San Francisco', pincode: 94101 }
  }
]
```

`Including and Excluding Fields Together:` You can use both inclusion and exclusion in the same projection. If a field is specified with both 1 and 0, it will be excluded.

Example: Include "name" and "email" fields but exclude "password" field:

```bash
db.users.find({}, { name: 1, email: 1, password: 0 })
```

`Projection on Nested Fields:` Projections can also be applied to fields within nested documents or arrays. You can specify the field path using dot notation.

Example: Include only the "address.city" field from a nested document:

```bash
db.customers.find({}, { "address.city": 1 })
```

Output

```mongosh +@output
> db.users.find({}, { "address.city": 1 })
[
  {
    _id: ObjectId("651e6260f3b5b884192b8f74"), address: { city: 'New York' }
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f75"), address: { city: 'Los Angeles' }
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f76"), address: {city: 'Madrid' }
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f77"), address: {city: 'Chicago' }
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f78"), address: { city: 'San Francisco' }
  }
]
```

`Limiting the Number of Results:` You can combine projections with other query options like limit() to further control the result set.

Example: Include only "name" and "email" fields and limit the result to 5 documents:

```bash
db.users.find({}, { name: 1, email: 1 }).limit(5)
```

Output

```mongosh +@output
> db.users.find({}, {name:1, email:1}).limit(3)
[
  {
    _id: ObjectId("651e6260f3b5b884192b8f74"),
    name: 'John Doe',
    email: john.doe@example.com'
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f75"),
    name: 'Alice Smith',
    email: alice.smith@example.com'
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f76"),
    name: 'Carlos Rodriguez',
    email: 'carlos.rodriguez@example.com'
  }
]
```

`Special Fields Exclusion:` MongoDB provides a way to exclude the \_id field by default when projecting fields. If you want to include the \_id field, you need to explicitly specify it in the projection.

Example: Exclude the \_id field from the result:

```bash
db.users.find({}, { _id: 0 })
```

`Using Projections for Performance Optimization:`

Projections are useful for optimizing query performance. By retrieving only the necessary fields, you reduce the amount of data transferred over the network and potentially improve query execution speed. This is especially important in scenarios where large datasets are involved.

Example: Exclude the "\_id" field from the query results

```bash
db.todos.find({}, { _id: 0 })
```

In this query, we exclude the "\_id" field from the results.

**Limiting Results and Paging:**

`Limiting Results:` Limiting results in MongoDB means restricting the number of documents returned by a query. You can use the limit() method to achieve this. Limiting results is useful when you want to retrieve only a subset of documents, such as the first N documents from a collection.

Example: Limiting Results

Suppose you have a "todos" collection with various tasks, and you want to retrieve only the first 5 tasks:

```bash
db.todos.find().limit(5)
```

Output

```mongosh +@output
> db.users.find().limit (2)
[
  {
    _id: ObjectId("651e6260f3b5b884192b8f74"),
    name: John Doe',
    email: john.doe@example.com' password: 'hashedpassword123',
    age: 30,
    address: { city: 'New York', pincode: 10001 }
  },
  {
    _id: ObjectId("651e6260f3b5b884192b8f75"),
    name: 'Alice Smith',
    email: 'alice.smith@example.com',
    age: 28, address: { city: 'Los Angeles', pincode: 90001 }
  }
]
```

`Paging:`

Paging, also known as pagination, is the process of dividing a large set of results into smaller, manageable chunks (pages) and allowing users to navigate through these pages. Paging is useful when you have a large dataset, and you want to display a limited number of records at a time.

In MongoDB, you can implement paging by combining the limit() and skip() methods. The skip() method allows you to skip a specified number of documents before returning the next set of results.

Example: Implementing Paging
Let's say you want to implement paging with 5 records per page. To retrieve the second page of tasks, you skip the first 5 tasks and then limit the results to 5:

```bash
// Skip the first 5 tasks (first page) and retrieve the next 5 tasks (second page)
db.todos.find().skip(5).limit(5)
```

Output

```mongosh +@output
> db.todos.find().skip(2).limit(2)
[
  {
    _id: ObjectId("651e5f4df3b5b884192b8f71"),
    task: 'Prepare for the presentation',
    completed: false,
    priority: High',
    tags: ['work' 'presentation' ],
    dueDate: 2023-09-20',
    category: 'Business'
  },
  {
    _id: ObjectId("651e5f4df3b5b884192b8f72"),
    task: 'Exercise for 30 minutes',
    completed: true,
    priority: 'Low',
    tags: ['health', 'exercise' ],
    dueDate: 2023-09-12',
    category: Personal'
  }
]
```

### Simple Updates and Deletes

Operations that modify the values of fields within documents in a collection. These updates can be performed on one or more documents and can change existing field values, add new fields, or remove existing fields. MongoDB provides various update operators and methods to perform these field updates.

MongoDB provides a set of update operators that allow you to perform specific modifications on fields within documents.

`MongoDB Update Methods:` You can perform field updates in MongoDB using update methods such as updateOne(), updateMany(), and findOneAndUpdate()

```bash
db.collection.updateOne(filter, update, options)
db.collection.updateMany(filter, update, options)
```

Example: Using $set to update a single document

```bash
db.todos.updateOne(
  { _id: ObjectId("5f9d9c9785f8a4e1f40922c6") },
  { $set: { completed: true } }
)
```

Output

```mongosh +@output
> db.todos.updateOne({ _id: ObjectId("651e5f4df3b5b884192b8f72") },{ $set: { completed: true } }
)
  {
    acknowledged: true,
    insertedId: null,
    matchedCount: 1,
    modifiedCount: 0,
    upsertedCount: 0
  }
```

Example: Using $inc to increment a numeric field in multiple documents

```bash
db.products.updateMany(
  { category: "Electronics" },
  { $inc: { price: 50 } }
)
```

Output

```mongosh +@output
> db.products.updateMany({ category: "Electronics" }, { $inc: { price: 50 } })
  {
    acknowledged: true,
    insertedId: null,
    matchedCount: 2,
    modifiedCount: 2,
    upsertedCount: 0
  }
```

`MongoDB Array Updates:` Field updates are also commonly used with arrays in MongoDB. You can add elements to arrays, remove elements, or modify specific array elements using update operators.

Example: Using $push to add an element to an array

```bash
db.users.updateOne(
  { _id: ObjectId("5f9d9c9785f8a4e1f40922c6") },
  { $push: { hobbies: "walking" } }
)
```

Output

```mongosh +@output
> db.users.updateOne({ _id: ObjectId("651e6260f3b5b884192b8f78")}, {$push: {hobbies: "walking"}})
  {
    acknowledged: true,
    insertedId: null,
    matchedCount: 1,
    modifiedCount: 1,
    upsertedCount: 0
  }
```

Example: Using $pull to remove elements from an array

```bash
db.orders.updateMany(
  { status: "completed" },
  { $pull: { items: { product: "Widget" } } }
)
```

Output

```mongosh +@output
> db.todos.updateMany ({status: completed}, {$pull: {items: {product: "Widget"}}})
  {
    acknowledged: true,
    insertedId: null,
    matchedCount: 4,
    modifiedCount: 0,
    upsertedCount: 0
  }
```

**Field Insertions and removals**

Ability to add new fields to existing documents or remove fields from documents in a collection. This flexibility is one of the advantages of using a NoSQL database like MongoDB, where documents within a collection can have different structures.

`Field Insertions:` Field insertions involve adding new fields to existing documents in a collection. You can add fields to one or more documents without affecting the structure of other documents in the same collection. This dynamic schema design allows you to accommodate new data requirements over time.

Example: Add a new field to a document

Suppose you have a "todos" collection with documents like this:

```bash
{
  "task": "Buy groceries",
  "completed": false
}
```

You can add a new field, such as "dueDate," to an existing document:

```bash
db.todos.updateOne(
  { task: "Buy groceries" },
  { $set: { dueDate: "2023-09-30" } }
)
```

Now, the document will look like this:

```bash
{
  "task": "Buy groceries",
  "completed": false,
  "dueDate": "2023-09-30"
}
```

`Field Removal:`

Field removal involves deleting a specific field from one or more documents in a collection. You can remove fields that are no longer needed, which helps keep your documents concise and reduces storage space.

Example: Remove a field from a document

Using the same "todos" collection, you can remove the "dueDate" field from a document:

```bash
db.todos.updateOne(
  { task: "Buy groceries" },
  { $unset: { dueDate: "" } }
)
```

After executing this query, the "dueDate" field will be removed from the document:

```bash
{
  "task": "Buy groceries",
  "completed": false
}
```

**Document Deletion**

`Deleting a Single Document:` To delete a single document that matches a specific condition, you can use the deleteOne() method. Here's an example:

Suppose we have a "todos" collection with the following documents:

```json
{
  _id: ObjectId("1"),
  task: "Buy groceries",
  completed: false
},
{
  _id: ObjectId("2"),
  task: "Finish project",
  completed: true
}

```

To delete the document with the task "Buy groceries," you can execute the following query:

```bash
db.todos.deleteOne({ task: "Buy groceries" })
```

Output

```mongosh +@output
> db.todos.deleteOne({task: "Read a book"})
{ acknowledged: true, deletedCount: 1 }
```

`Deleting Multiple Documents:` To delete multiple documents that match specific criteria, you can use the deleteMany() method. Here's an example:

Suppose you want to delete all completed tasks from the "todos" collection:

```bash
db.todos.deleteMany({ completed: true })
```

Output

```mongosh +@output
> db.todos.deleteMany({completed:true})
{ acknowledged: true, deletedCount: 3 }
```

`Deleting All Documents in a Collection:` If you want to delete all documents in a collection, you can use the deleteMany() method without specifying any criteria:

```bash
db.todos.deleteMany({})
```

Output

```mongosh +@output
> db.todos.deleteMany ({})
{ acknowledged: true, deletedCount: 1 }
```

`Deleting Documents by ObjectId:` You can also delete documents by their \_id field, which is typically an ObjectId. For example, to delete a document with a specific ObjectId, you can use the deleteOne() method as follows:

```bash
db.todos.deleteOne({ _id: ObjectId("1") })
```

Output

```mongosh +@output
>db.todos.deleteOne({ _id: ObjectId("1") })
{ acknowledged: true, deletedCount: 1 }
```

`Handling Deletion Errors:` It's important to note that MongoDB will not throw an error if a deletion operation does not find a matching document. The operation will simply have no effect. Therefore, it's a good practice to check the result of deletion operations to ensure they have deleted the intended documents.

Here's an example of checking the result of a deletion operation:

```js
const result = db.todos.deleteOne({ task: "Non-existent task" });

if (result.deletedCount === 1) {
  print("Document deleted successfully.");
} else {
  print("No matching document found for deletion.");
}
```

### More Complex Types of Queries

Sample data

Articles:

```json
{
  "author": "Alice",
  "comments": [
    {
      "commenter": "Bob",
      "text": "Great article! Thanks for sharing."
    },
    {
      "commenter": "Carol",
      "text": "I found this very informative."
    },
    {
      "commenter": "David",
      "text": "Looking forward to more articles from you!"
    }
  ]
},
{
  "author": "Eve",
  "comments": [
    {
      "commenter": "Frank",
      "text": "Excellent read!"
    }
  ]
},
{
  "author": "Grace",
  "comments": []
}
```

**Existential Field Values**

Refer to the presence or absence of a field within a document. MongoDB provides operators to query documents based on whether a field exists, doesn't exist, or has a specific value. This is particularly useful when dealing with flexible or schema-less data structures

`1. $exists Operator:` The $exists operator is used to check whether a field exists within a document. It takes a boolean value, either true or false, to indicate whether the field should exist or not.

Example 1: Find documents where the "comments" field exists:

```bash
db.articles.find({ comments: { $exists: true } })
```

Output

```mongosh +@output
> db.articles.find({ comments: { $exists: true } })
[
  {
    _id: ObjectId("651e9600f3b5b884192b8f81"), author: 'Alice',
    comments: [
    { commenter: 'Bob', text: 'Great article! Thanks for sharing.' },
    { commenter: 'Carol', text: 'I found this very informative.' },
    { commenter: 'David' }
    ]
  },
  {
    _id: ObjectId("651e9600f3b5b884192b8f82"), author: 'Eve',
    comments: [ {'commenter: 'Frank', text: 'Excellent read!' } ]
  },
]
```

Example 2: Find documents where the "author" field does not exist:

```bash
db.articles.find({ author: { $exists: false } })
```

Output

```mongosh +@output
>db.articles.find({ author: { $exists: false } })
  {
    _id: ObjectId("651e9600f3b5b884192b8f83"),
    comments: []
  }
```

`2. $type Operator:` The $type operator allows you to query documents based on their BSON data type. You can specify the data type as a number or a string representing the BSON data type.

Example 3: Find documents where the "brand" field is of type string:

```bash
db.scores.find({ brand: { $type: "string" } })
```

Output

```mongosh +@output
> db.products.find({ brand: { $type: "string" } })
[
  {
    _id: ObjectId("651e627df3b5b884192b8f7a"), name: 'Smartphone',
    category: 'Electronics',
    price: 649.99,
    in_stock: true,
    brand: Samsung',
    model: Galaxy S21',
    color: 'Phantom Black'
  },
  {
    _id: ObjectId("651e627df3b5b884192b8f7c"), name: "Men's Jeans",
    category: 'Clothing',
    price: 49.99,
    in_stock: false,
    brand: "Levi's",
    size: 32W x 34L',
    color: 'Dark Blue',
  },
  {
    _id: ObjectId("651e627df3b5b884192b8f7d"), name: 'Coffee Maker',
    category: 'Appliances',
    price: 79.99,
    in_stock: true,
    brand: 'Keurig',
    type: 'Single Serve'
  }
]
```

Example 4: Find documents where the "description" field is of type string:

```bash
db.products.find({ description: { $type: 2 } })
```

`3. Combining $exists and $type:` You can combine the $exists and $type operators to perform more complex queries based on the existence and data type of a field.

Example 5: Find documents where the "category" field exists and is of type string:

```bash
db.users.find({ email: { $exists: true, $type: "string" } })
```

Output

```mongosh +@output
> db.products.find({category: {$exists: true, $type: "string"}})
[
  {
    _id: ObjectId("651e627df3b5b884192b8f79"),
    name: 'Laptop',
    category: 'Electronics',
    price: 1049.99,
    in_stock: true
  };
  {
    _id: ObjectId("651e627df3b5b884192b8f7b"), name: The Great Gatsby',
    category: 'Books'
    price: 14.99,
    in_stock: true,
    author: 'F. Scott Fitzgerald',
    genre: Classic Fiction'
  },
  {
    name: "Men's Jeans",
    _id: ObjectId("651e627df3b5b884192b8f7c"),
    category: 'Clothing',
    in_stock: false,
    price: 49.99,
    brand: "Levi's",
    size: 32W x 34L',
    color: 'Dark Blue'
  },
  {
    _id: ObjectId("651e627df3b5b884192b8f7d"), name: 'Coffee Maker',
    category: 'Appliances',
    price: 79.99,
    in_stock: true,
    brand: 'Keurig',
    type: Single Serve'
  }
]
```

Existential field value queries are useful for handling data where not all documents have the same fields or where fields may have different data types. MongoDB's flexible schema allows you to work with data in a dynamic and adaptable way.

### Aggregations and groups

Refer to the process of performing data transformations and analysis on documents within a collection. MongoDB's aggregation framework provides powerful tools for grouping, filtering, and processing data to derive meaningful insights. This feature is especially valuable when you need to perform complex operations on your data.

MongoDB's aggregation framework uses the concept of an aggregation pipeline. The pipeline consists of stages, and each stage performs a specific data transformation or operation on the input data (documents) before passing it to the next stage. The output of one stage becomes the input of the next stage.

A typical aggregation pipeline may consist of stages like $match, $group, $project, $sort, and more, depending on your requirements.

`Example 1: Grouping and Counting:`

Let's say you have a collection of orders and you want to group the orders by the product they contain and count how many times each product appears in the orders.

```bash
db.orders.aggregate([
  {
    $group: {
      _id: "$product",
      totalQuantity: { $sum: 1 }
    }
  }
])
```

Output

```mongosh +@output
> db.orders. aggregate([{$group: {_id: "$product", totalQuantity: {$sum: 1}}}])
[
  { _id: 'Laptop', totalQuantity: 6 },
  { _id: 'Tablet', totalQuantity: 8 }
]
```

In this example, the $group stage groups documents by the "product" field, and the $sum operator counts the number of documents in each group. The result will show how many times each product appears.

`Example 2: Filtering and Sorting:`

You might want to find the highest-priced product in each category. You can achieve this by filtering the documents and then sorting them.

```bash
db.products.aggregate([
  {
    $match: {
      category: "Electronics"
    }
  },
  {
    $sort: {
      price: -1
    }
  },
  {
    $group: {
      _id: "$category",
      highestPriceProduct: { $first: "$name" }
    }
  }
])
```

Output

```mongosh +@output
[
  {
    _id: 'Electronics',
    highestPriceProduct: 'High-End Laptop Model XYZ'
  }
]
```

In this example, we use the $match stage to filter documents in the "Electronics" category. Then, we $sort the filtered documents by price in descending order and use the $group stage to find the highest-priced product in each category.

`Example 3: Projecting Fields:`

You can use the $project stage to reshape the output documents by specifying which fields to include or exclude.

```bash
db.customers.aggregate([
  {
    $project: {
      _id: 0, // Exclude the _id field
      fullName: { $concat: ["$firstName", " ", "$lastName"] }
    }
  }
])
```

Output

```mongosh +@output
[ { fullName: 'Emily Davis' }, { fullName: 'Sarah Brown' } ]
```

In this example, we use $project to create a new field called "fullName" by concatenating the "firstName" and "lastName" fields and exclude the \_id field.

`Example 4: Unwinding Arrays:`

If your documents contain arrays and you want to treat the array elements as separate documents, you can use the $unwind stage.

```bash
db.orders.aggregate([
  {
    $unwind: "$items"
  }
])
```

Output

```mongosh +@output
[
  {
    _id: ObjectId("5fbdac71a2b7e7429a31c8a1"), orderNumber: 'ORD123456',
    customerName: John Doe',
    items: { productName: Widget A', quantity: 5, unitPrice: 10.99 }
  },
  {
    orderNumber: 'ORD123456',
    customerName: John Doe',
    items: { productName: Widget B', quantity: 3, unitPrice: 15.99 }
  }
]
```

Here, the $unwind stage splits the "items" array into separate documents, creating one document for each item in the array.

`Example 5: Aggregating Nested Fields:`

You can perform aggregations on nested fields within documents.

```bash
db.sales.aggregate([
  {
    $unwind: "$products"
  },
  {
    $group: {
      _id: "$products.category",
      totalRevenue: { $sum: "$products.price" }
    }
  }
])
```

Output

```mongosh +@output
[
  { _id: 'Electronics', totalRevenue: 3500 },
  { _id: 'Clothing', totalRevenue: 1250 },
  { _id: 'Appliances', totalRevenue: 2200 }
]
```

In this example, we first $unwind the "products" array and then group the documents by the "category" field within the nested "products" field to calculate the total revenue for each category.

### Aggregations and groups in heirarchical data

Aggregations and grouping in hierarchical data are important operations in MongoDB when dealing with structured and nested data. Hierarchical data is often organized in a parent-child relationship, and you may need to perform aggregations and grouping to analyze or manipulate this data effectively. MongoDB provides powerful aggregation pipelines and grouping capabilities to address these requirements.

MongoDB's Aggregation Framework is a versatile tool for performing data transformation and analysis. It allows you to filter, project, group, and reshape data in a structured manner. When dealing with hierarchical data, you can use the Aggregation Framework to navigate and aggregate nested structures.

Example: Aggregating Nested Data

Consider a collection of "departments" where each department has employees, and each employee has sales data:

```bash
{
  _id: 1,
  name: "HR",
  employees: [
    { name: "Alice", sales: 1000 },
    { name: "Bob", sales: 800 }
  ]
}
{
  _id: 2,
  name: "Sales",
  employees: [
    { name: "Charlie", sales: 1500 },
    { name: "David", sales: 1200 }
  ]
}

```

You can use the Aggregation Framework to find the total sales per department:

```bash
db.departments.aggregate([
  {
    $unwind: "$employees"
  },
  {
    $group: {
      _id: "$name",
      totalSales: { $sum: "$employees.sales" }
    }
  }
])

```

Output

```mongosh +@output
[
  {
    "_id": "HR",
    "totalSales": 1800
  },
  {
    "_id": "Sales",
    "totalSales": 2700
  }
]
```

In this example, we first unwind the "employees" array to transform it into separate documents, then we group by department name and calculate the total sales using the $sum operator.

`Grouping:` Grouping is an essential operation for summarizing data based on specific criteria, especially when working with hierarchical data.

Example: Grouping by Category

Consider a collection of "products" with categories:

```bash
{
  _id: 1,
  name: "Laptop",
  category: "Electronics",
  price: 1000
}
{
  _id: 2,
  name: "Book",
  category: "Books",
  price: 20
}
{
  _id: 3,
  name: "Smartphone",
  category: "Electronics",
  price: 500
}
```

You can group products by category and calculate the average price for each category:

```bash
db.products.aggregate([
  {
    $group: {
      _id: "$category",
      avgPrice: { $avg: "$price" }
    }
  }
])
```

Output

```mongosh +@output
[
  { _id: 'Electronics', avgPrice: 750 },
  { _id: 'Books', avgPrice: 20 }
]
```

In this query, we group products by the "category" field and calculate the average price using the $avg operator.

`Hierarchical Data Aggregation:` Hierarchical data often involves nested structures. MongoDB's Aggregation Framework can handle such data with ease.

Example: Aggregating Nested Categories

Consider a collection of "categories" where each category can have subcategories:

```bash
{
  _id: 1,
  name: "Electronics",
  subcategories: [
    { name: "Laptops" },
    { name: "Smartphones" }
  ]
}
{
  _id: 2,
  name: "Books",
  subcategories: [
    { name: "Fiction" },
    { name: "Non-Fiction" }
  ]
}
```

You can aggregate and flatten this hierarchical data to get a list of all subcategories:

```bash
db.categories.aggregate([
  {
    $unwind: "$subcategories"
  },
  {
    $project: {
      _id: 0,
      categoryName: "$name",
      subcategoryName: "$subcategories.name"
    }
  }
])
```

Output

```mongosh +@output
[
  { categoryName: 'Electronics',
  subcategoryName: 'Laptops'
  },
  { categoryName: 'Electronics',
  subcategoryName: 'Smartphones'
  },
  { categoryName: 'Books',
  subcategoryName: 'Fiction'
  },
  { categoryName: 'Books',
  subcatergoryName: 'Non-Fiction'
  }
]
```

In this example, we unwind the "subcategories" array and project the data to flatten it, resulting in a list of all subcategories.

### MapReduce

MapReduce is a powerful data processing paradigm used in MongoDB to perform complex data aggregations and transformations on large datasets. It consists of two main stages: the "Map" stage and the "Reduce" stage. MapReduce is especially useful for tasks that require grouping, filtering, and summarizing data.

**MapReduce Phases:**
`1. Map Phase:`

- In this phase, the input data is divided into chunks.
- A JavaScript function (the "map" function) is applied to each chunk, creating a set of key-value pairs.
- The "map" function is responsible for selecting and transforming the data as needed.
- The output of the "map" phase is an intermediate collection of key-value pairs.

`2. Reduce Phase:`

- In this phase, the key-value pairs produced by the "map" phase are grouped by their keys.
- A JavaScript function (the "reduce" function) is applied to each group of key-value pairs.
- The "reduce" function aggregates, summarizes, or processes the data within each group.
- The output of the "reduce" phase is the final result.

Example: Word Count using MapReduce:
Let's consider a simple example of counting words in a collection of documents.

Map Function:

```js
var mapFunction = function () {
  var text = this.text; // Assuming the document has a "text" field
  var words = text.split(" ");
  for (var i = 0; i < words.length; i++) {
    emit(words[i], 1); // Emit each word as a key with a count of 1
  }
};
```

Reduce Function:

```js
var reduceFunction = function (key, values) {
  return Array.sum(values); // Sum the counts for each word
};
```

Running MapReduce:

```bash
db.documents.mapReduce(
  mapFunction,
  reduceFunction,
  { out: "word_count" }
)
```

Output

```mongosh +@output
[
  { "_id": "This", "value": 2 }
  { "_id": "is", "value": 1 }
  { "_id": "object", "value": 1 }
  { "_id": "sample", "value": 1 }
  { "_id": "document", "value": 3 }
  { "_id": "with", "value": 1 }
  { "_id": "some", "value": 1 }
  { "_id": "words.", "value": 1 }
]
```

In this example, we use MapReduce to count the occurrences of each word in a collection of documents. The "map" function splits the text into words and emits each word with a count of 1. The "reduce" function then sums the counts for each word. The result is stored in a new collection called "word_count."

**Use Cases for MapReduce in MongoDB:**

1. `Aggregation:` Summarizing data by grouping and aggregating values.
2. `Data Cleaning:` Transforming and cleaning data during the Map phase.
3. `Text Analysis:` Analyzing and processing text data, such as counting words or extracting keywords.

Complex Calculations: Performing complex calculations that cannot be achieved with simple queries.
While MapReduce is a powerful tool, it's worth noting that it involves JavaScript execution, which can be slower than some other aggregation methods. As a result, MongoDB introduced the Aggregation Framework, which is often more efficient for many aggregation tasks. However, MapReduce remains a valuable option for scenarios that require custom data processing and transformations.

**Types of logic that can be expressed as MapReduce declarations**

`1. Aggregation:` MapReduce can be used to perform aggregation operations like sum, count, average, minimum, maximum, and more. You can group and aggregate data based on specific criteria.

Example: Calculate the total sales per product category

```js
// Map function
var mapFunction = function () {
  emit(this.category, this.sales);
};

// Reduce function
var reduceFunction = function (key, values) {
  return Array.sum(values);
};

db.sales.mapReduce(mapFunction, reduceFunction, { out: "category_sales" });
```

Output

```mongosh +@output
[
  {
    "_id": "Electronics",
    "value": 3500
  },
  {
    "_id": "Clothing",
    "value": 1200
  },
  {
    "_id": "Books",
    "value": 800
  }
]
```

`2. Filtering:`

MapReduce can filter data based on specific conditions, allowing you to include or exclude documents in the result set.

Example: Calculate the average price of expensive products

```js
// Map function
var mapFunction = function () {
  if (this.price > 100) {
    emit("expensive", this.price);
  }
};

// Reduce function
var reduceFunction = function (key, values) {
  return Array.avg(values);
};

db.products.mapReduce(mapFunction, reduceFunction, {
  out: "average_expensive_price",
});
```

Output

```mongosh +@output
[
  {
    "_id": "expensive",
    "value": 587
  }
]

```

`3. Data Transformation:` MapReduce can transform data into a different format or structure that better suits your needs.

Example: Transform product data into a list of product names by category

```js
// Map function
var mapFunction = function () {
  emit(this.category, [this.name]);
};

// Reduce function
var reduceFunction = function (key, values) {
  return Array.concat(...values);
};

db.products.mapReduce(mapFunction, reduceFunction, {
  out: "products_by_category",
});
```

Output

```mongosh +@output
[
  {
    "_id": "Clothing",
    "value": ["T-Shirt", "Jeans"]
  },
  {
    "_id": "Electronics",
    "value": ["Laptop", "Smartphone", "Camera"]
  }
]

```

`4. Text Analysis:` MapReduce can be used for text analysis tasks, such as word frequency counting, sentiment analysis, and more.

Example: Calculate word frequency in a collection of text documents

```js
// Map function
var mapFunction = function () {
  var words = this.text.split(" ");
  for (var i = 0; i < words.length; i++) {
    emit(words[i], 1);
  }
};

// Reduce function
var reduceFunction = function (key, values) {
  return Array.sum(values);
};

db.text_documents.mapReduce(mapFunction, reduceFunction, {
  out: "word_frequency",
});
```

Output

```mongosh +@output
[
  { "_id": "The", "value": 2 },
  { "_id": "quick", "value": 1 },
  { "_id": "brown", "value": 2 },
  { "_id": "fox", "value": 1 },
  { "_id": "jumps", "value": 1 },
  { "_id": "over", "value": 1 },
  { "_id": "the", "value": 1 },
  { "_id": "lazy", "value": 1 },
  { "_id": "dog.", "value": 1 },
  { "_id": "A", "value": 1 },
  { "_id": "cat", "value": 1 },
  { "_id": "chases", "value": 1 },
  { "_id": "a", "value": 2 },
  { "_id": "white", "value": 1 },
  { "_id": "mouse.", "value": 1 },
  { "_id": "escapes", "value": 1 },
  { "_id": "into", "value": 1 },
  { "_id": "small", "value": 1 },
  { "_id": "burrow.", "value": 1 }
]

```

`5. Custom Aggregations:` You can implement custom aggregation logic that may not be easily achievable with standard aggregation operators.

Example: Calculate the weighted average of student scores

```js
// Map function
var mapFunction = function () {
  emit(this.subject, {
    totalScore: this.score,
    weight: this.weight,
  });
};

// Reduce function
var reduceFunction = function (key, values) {
  var result = {
    totalScore: 0,
    weight: 0,
  };

  for (var i = 0; i < values.length; i++) {
    result.totalScore += values[i].totalScore;
    result.weight += values[i].weight;
  }

  return result;
};

db.student_scores.mapReduce(mapFunction, reduceFunction, {
  out: "weighted_average_scores",
});
```

Output

```mongosh +@output
[
  {
    "_id": ObjectId("..."),
    "product": "Product A",
    "quantity": 10,
    "price": 50.0,
    "year": 2023,
    "month": 10
  },
  {
    "_id": ObjectId("..."),
    "product": "Product B",
    "quantity": 5,
    "price": 30.0,
    "year": 2023,
    "month": 9
  },
  {
    "_id": ObjectId("..."),
    "product": "Product A",
    "quantity": 8,
    "price": 50.0,
    "year": 2023,
    "month": 10
  },
  {
    "_id": ObjectId("..."),
    "product": "Product C",
    "quantity": 15,
    "price": 20.0,
    "year": 2023,
    "month": 9
  }
]
```

**Mapping documents**

Suppose you have a "sales" collection with documents representing sales transactions, and each document has the following structure:

```json
{
  "_id": 1,
  "date": "2023-09-01",
  "product": "Widget A",
  "quantity": 10,
  "price": 20
}
```

1. Calculating Total Sales for Each Product:

You want to calculate the total sales amount for each product. You can use the $group stage to group documents by the "product" field and calculate the sum of the "quantity" multiplied by the "price" for each group.

```bash
db.sales.aggregate([
  {
    $group: {
      _id: "$product",
      totalSales: { $sum: { $multiply: ["$quantity", "$price"] } }
    }
  }
])
```

The result will provide the total sales for each product:

```json
[
  { "_id": "Widget A", "totalSales": 200 },
  { "_id": "Widget B", "totalSales": 150 }
  // ...
]
```

2. Extracting Year and Month from Date:

You want to analyze sales trends by year and month. You can use the $project stage to extract the year and month from the "date" field.

```bash
db.sales.aggregate([
  {
    $project: {
      year: { $year: { $dateFromString: { dateString: "$date" } } },
      month: { $month: { $dateFromString: { dateString: "$date" } } },
      product: 1,
      quantity: 1,
      price: 1
    }
  }
])
```

The result will include the "year" and "month" fields:

```json
[
  {
    "year": 2023,
    "month": 9,
    "product": "Widget A",
    "quantity": 10,
    "price": 20
  },
  {
    "year": 2023,
    "month": 9,
    "product": "Widget B",
    "quantity": 8,
    "price": 15
  }
  // ...
]
```

3. Filtering Documents:

You want to analyze sales data for a specific product. You can use the $match stage to filter documents based on the "product" field.

```bash
db.sales.aggregate([
  {
    $match: { product: "Widget A" }
  },
  {
    $group: {
      _id: "$product",
      totalSales: { $sum: { $multiply: ["$quantity", "$price"] } }
    }
  }
])
```

The result will provide the total sales for "Widget A" only:

```json
[{ "_id": "Widget A", "totalSales": 200 }]
```

**Reducing Values**

Refers to the process of aggregating and summarizing data from multiple documents in a collection into a single result. MongoDB provides a powerful aggregation framework that allows you to perform complex data reduction operations, such as grouping, filtering, and transforming data.

`1. Aggregation Pipeline:` MongoDB's aggregation pipeline is a series of data processing stages that documents pass through. Each stage performs a specific operation on the input documents and passes the results to the next stage. The aggregation pipeline allows you to build complex data reduction workflows.

`2. Operators:` MongoDB provides a wide range of aggregation operators that you can use within the aggregation pipeline to perform various data reduction operations. Some commonly used aggregation operators include $match, $group, $project, $unwind, and $sum, among others

`3. Grouping:` The $group operator is used to group documents by one or more fields and perform aggregation operations within each group. This is useful for calculating sums, averages, counts, and other aggregated values.

`4. Filtering:` The $match operator allows you to filter documents based on specified criteria before passing them to the next stage of the aggregation pipeline. It's similar to the find() method but operates within the pipeline

`5. Transformation:` The $project operator is used to reshape documents, rename fields, or include/exclude specific fields in the output. It's useful for creating custom views of the data.

Example: Aggregating Sales Data
Let's consider an example where you have a collection of sales transactions and you want to reduce the data to calculate the total sales revenue for each product category. Here's how you can do it using MongoDB's aggregation framework:

```bash
db.sales.aggregate([
  {
    $group: {
      _id: "$productCategory",
      totalSales: { $sum: "$amount" }
    }
  },
  {
    $project: {
      productCategory: "$_id",
      totalSales: 1,
      _id: 0
    }
  }
])
```

Output

```mongosh +@output
[
  { _id: 'English', value: { totalScore: 88, weight: 0.3 } },
  { _id: 'History', value: { totalScore: 75, weight: 0.4 } }
]
```

In this example:

- We use the $group stage to group documents by the "productCategory" field and calculate the total sales within each group using the $sum operator.

- In the $project stage, we reshape the output to include the "productCategory" and "totalSales" fields while excluding the default "\_id" field.

The result will be a list of product categories along with their total sales revenue, which is a reduced representation of the original data.

Reducing values in MongoDB allows you to extract meaningful insights from your data, perform calculations, and generate aggregated reports—all within the database, which can be highly efficient for large datasets. The flexibility and power of the aggregation framework make it a valuable tool for data analysis and reporting in MongoDB

### Sharding

**Configuring replication**

Configuring replication in MongoDB is a fundamental aspect of creating a highly available and fault-tolerant database system. Replication involves maintaining multiple copies of your data across multiple servers or nodes, which ensures data redundancy and fault tolerance. While sharding is related to distributing data across multiple servers to improve performance and scalability, it's separate from replication.

Replication in MongoDB is the process of creating and maintaining copies of your data on multiple servers, with one server designated as the primary and others as secondaries. This setup provides the following benefits:

1. `High Availability:` If the primary node fails, one of the secondaries can be automatically promoted as the new primary, minimizing downtime.

2. `Data Redundancy:` Data is replicated across multiple nodes, ensuring that there are copies available in case of data loss or hardware failures.

3. `Load Balancing:` Read operations can be distributed across secondary nodes, improving overall system performance.

4. `Data Locality:` Replication allows you to place copies of data closer to users or in different geographic regions, improving data access speed.

To configure replication in MongoDB, you need to follow these steps:

1. `Start MongoDB Instances:` Ensure you have multiple MongoDB instances running on different servers, each with a unique --port and --dbpath (data directory).

2. `Initialize the Primary Node:` Connect to one of the MongoDB instances (the one you want to be the primary) and run the rs.initiate() command to initiate replication on the primary node.

3. `Add Secondary Nodes:` Add secondary nodes to the replica set using the rs.add() command, specifying the server addresses.

4. `Verify Configuration:` Use the rs.status() command to check the status of your replica set.

5. `Configure Replication Settings:` You can configure additional replication settings such as write concern and read preferences.

6. `Failover Handling:` MongoDB handles failovers automatically if the primary node goes down.

Sharding is a different concept from replication, although both contribute to creating a scalable and highly available MongoDB deployment. Sharding is used when your data grows to the point where a single MongoDB instance can no longer handle it. It involves distributing your data across multiple servers or shards, each responsible for a portion of the data.

Here's how sharding works:

1. `Shard Key:` You choose a field (the shard key) to determine how data is distributed across shards. MongoDB uses this key to determine which shard should handle each document.

2. `Shard Servers:` Shards are separate MongoDB instances or clusters. Each shard contains a subset of your data.

3. `Config Servers:` There are also config servers that store metadata about how data is distributed across shards.

4. `Router (mongos):` An application connects to a router (mongos), which routes queries and updates to the appropriate shard(s) based on the shard key.

Sharding is useful for horizontally scaling your MongoDB database to handle large amounts of data and high traffic loads.

In practice, you often use both replication and sharding to create a highly available, scalable, and fault-tolerant MongoDB infrastructure. Replication ensures that each shard has its own replicated copy, enhancing data availability within each shard.

Here's a simplified example of how to enable sharding for a MongoDB collection:

1. Enable sharding for a database:

```bash
use admin
db.runCommand({ enableSharding: "mydb" })
```

2. Choose a shard key and shard the collection:

```bash
use mydb
db.createCollection("mycollection")
db.mycolleciton.createIndex({ shardKeyField: 1 })
sh.shardCollection("mydb.mycollection", { shardKeyField: 1 })
```

Remember that sharding requires careful planning and monitoring to ensure an even distribution of data and optimal performance.

**Configuring sharding**

Here are the steps to configure sharding in MongoDB:

Step 1: Set Up a Sharded Cluster

1. Start multiple MongoDB instances (shards) on separate servers or virtual machines. You can specify different ports for each instance.

2. Start at least three config servers, which will store configuration data for the sharded cluster.

Step 2: Enable Sharding on the Database

In your MongoDB shell, connect to one of the shard servers and issue the following command to enable sharding on your database

```bash
use yourDatabase
sh.enableSharding("yourDatabase")
```

Step 3: Choose a Sharding Key

Select a field in your data to be the sharding key. The sharding key determines how data is distributed across the shards. For example, if you have a collection of user data, you might choose the "user_id" field as the sharding key.

```bash
db.yourCollection.ensureIndex({ "shardingKeyField": 1 })
```

Step 4: Add Shards to the Cluster

In your MongoDB shell, connect to one of the config servers and issue the following command to add a shard to the cluster:

```bash
sh.addShard("shard1Server:port")
```

Step 5: Enable Sharding on the Collection

Enable sharding on the collection using the sharding key:

```bash
sh.shardCollection("yourDatabase.yourCollection", { "shardingKeyField": 1 })
```

Step 6: Distribute Data

As you insert data into the collection, MongoDB will automatically distribute the data across the shards based on the sharding key.

Step 7: Query and Manage Data

You can now query and manage your sharded data using the Mongos router. Connect to Mongos from your application, and it will route queries and data requests to the appropriate shard based on the sharding key.

Example:

Suppose you have a collection of user data that you want to shard based on the "user_id" field. Here's how you would configure sharding:

```bash
use mydb
sh.enableSharding("mydb")
db.users.ensureIndex({ "user_id": 1 })
sh.addShard("shard1.example.com:27017")
sh.shardCollection("mydb.users", { "user_id": 1 })
```

**Accessing clustered data from client APIs**

Before diving into accessing clustered data, let's briefly review the key components of MongoDB sharding:

1. `Shards:` These are individual MongoDB servers that store a subset of the data. Shards distribute data across the cluster.

2. `Shard Key:` A shard key is a field or a combination of fields chosen to determine how data is distributed across shards. It's essential to choose an appropriate shard key for even data distribution.

3. `Router (mongos):` The router is a routing service that directs client requests to the appropriate shard(s). Client applications connect to routers to access data.

4. `Config Servers:` These servers store metadata about the sharded cluster's configuration, such as the mapping between chunks of data and the shards.

When accessing data in a sharded MongoDB cluster from a client application, you need to consider the following points:

1. `Using the Router (mongos):` Client applications should connect to the mongos instances, which act as query routers. Mongos directs queries and commands to the appropriate shard(s) based on the shard key.

2. `Shard Key Awareness:` Client applications need to be shard key-aware. This means that queries should include the shard key whenever possible to ensure that queries are routed efficiently to the relevant shards. Queries without the shard key may result in scatter-gather queries across multiple shards, which can be less efficient.

3. `Scalability:` As the amount of data increases, MongoDB's sharding feature allows you to scale horizontally by adding more shards to the cluster. Client applications should be designed to take advantage of this scalability by distributing queries across multiple shards.

Example:

Let's consider a simple example using a sharded MongoDB cluster for storing user data. Assume you have a user collection with a shard key based on the "country" field. Each shard contains user data for a specific country.

```js
const MongoClient = require("mongodb").MongoClient;

const uri = "mongodb://mongos1:27017,mongos2:27017,mongos3:27017/mydb";

MongoClient.connect(uri, { useNewUrlParser: true }, (err, client) => {
  if (err) {
    console.error("Error connecting to mongos:", err);
    return;
  }

  const db = client.db("mydb");
  const usersCollection = db.collection("users");

  // Access data using the shard key for efficient routing
  const query = { country: "USA" };
  usersCollection.find(query).toArray((err, result) => {
    if (err) {
      console.error("Error querying data:", err);
      return;
    }

    console.log("Users from USA:", result);
    client.close();
  });
});
```

In this example, the client application connects to a mongos router. It then performs a query based on the shard key ("country") to efficiently route the query to the appropriate shard containing user data for the specified country.

**Latency and consistency in replicated and sharded MongoDB**

Replication in MongoDB involves maintaining multiple copies (replica set) of the same data across different servers or nodes. Each replica set typically consists of a primary node and one or more secondary nodes. Latency can be influenced by several factors in this setup:

1. `Read and Write Operations:` Latency varies for read and write operations. Read operations can be distributed to secondary nodes, which can reduce latency for read-heavy workloads. However, write operations are primarily directed to the primary node.

2. `Network Latency:` Network latency between nodes can affect data replication. If nodes are geographically distributed, network latency may be higher, impacting the time it takes for data to replicate from the primary to secondary nodes.

3. `Oplog Size and Replication Delay:` The Oplog (Operation Log) in MongoDB records write operations. Secondary nodes use the Oplog to catch up with the primary. If the Oplog size is small or if secondary nodes are lagging behind due to resource constraints, replication delays can occur.

4. `Load Balancing:` Proper load balancing of read operations across secondary nodes can help distribute the load and reduce latency.

Example:
Suppose you have a MongoDB replica set with a primary node in one data center and two secondary nodes in different data centers. If a read operation is directed to a secondary node closer to the user, it can result in lower latency compared to querying the primary node located farther away.

MongoDB offers different levels of data consistency in a replica set:

1. `Strong Consistency:` Read operations from secondary nodes return data that has been successfully replicated to a majority of nodes, ensuring strong consistency. However, strong consistency can increase read latency.

2. `Eventual Consistency:` Read operations from secondary nodes may return data that has not yet been replicated to a majority of nodes, providing eventual consistency with potentially lower read latency.

Latency in Sharded MongoDB:

In a sharded MongoDB cluster, data is distributed across multiple shards (individual MongoDB instances). Each shard can have its own replica set for high availability. Latency considerations in sharded setups include:

1. `Shard Key Design:` The choice of shard key can impact query latency. A well-chosen shard key can distribute data evenly across shards, reducing query latency.

2. `Balancing Data:` MongoDB's balancer redistributes chunks of data across shards to ensure even data distribution. This balancing process can affect latency if not managed properly.

3. `Query Routing:` Query routing decisions made by the query router (mongos) can influence query latency. It's crucial to ensure efficient routing.

Example:
Suppose you have a sharded MongoDB cluster with three shards. Properly distributed data across shards based on a well-designed shard key can result in lower query latency for specific queries as they target the appropriate shard with relevant data.

Consistency in Sharded MongoDB:

In a sharded setup, data consistency is often maintained at the shard level. Each shard may consist of a replica set to ensure high availability and data consistency within that shard.

Example:
If you perform a read operation against a specific shard, you'll get consistent results based on the data in that shard. However, querying multiple shards simultaneously may introduce eventual consistency, depending on the sharding configuration and replication settings.

## Project

### NPM packages

**dotenv**

`Installation:` `npm install dotenv`

`Purpose:` Injects environment variables into application code. Enables us to read configrations from `.env` file. Based on the environment(dev, testing or production) we are in we can load environment specific cofigs like port number, database connection url or db credentials.

`Usage:` import the package using `require("dotenv/config")`. Dont have to initialise a variable to store the module. Just requiring is enough. Place all out environment variables into a `.env` file in the root folder of out project.

```test
PORT=8080

JWT_SECRET = nodejstraining
USER_TOKEN_EXPIRY=3600
ADMIN_EMAIL=admin@nodejs.com

DATABASE_URL=mongodb://0.0.0.0:27017/todoapp
```

This is just a text file. No need to wrap strings like db connection url into quotes. Now we read the value within the application code using `process.env.PORT`. process is exposed by node.js. We can access all the environment variables from .env file using this.

**mongoose**

`Installation: ` `npm install mongoose`

`Purpose: ` Mongoose is a mongodb ODM(Object Document Mapper). Similar to ORM(Object Relational Mapper) in SQL. This is a client to interact with Mongodb. It exposes apis to write queries in programatically and handle in our routes instead from shell.

`Usage:` Create a model/schema of the collection. For example todo.

```js
const mongoose = require("mongoose");
const Schema = mongoose.Schema;
const todoSchema = new Schema(
  {
    task: {
      type: String,
      required: true,
    },
    isComplete: {
      type: Boolean,
      required: true,
      default: false,
    },
    user: { type: Schema.Types.ObjectId, ref: "User" },
  },
  {
    timestamps: true,
  }
);
module.exports = mongoose.model("Todo", todoSchema);
```

Create a model and export it. We can import this model in our route handler functions to perform secific actions. If we want to get all the todoes present in the database we can do so using the below line of code.

```js
const todos = await Todo.find({});
```

**zod**

`Installation:` `npm install zod`;
`Purpose:` zod is a validator. We cannot trust the data sent by the client. So backend needs to validate whether the data sent is as per requiement or not. If wrong type of data is sent or no data is sent, backend should respond with a `Bad request(400)`.

`Usage:` We can define the shape of the object we are expecting. In the below example we are expecting 2 fields `task` and `isComplete` in the request body. We can specify what error message to display when a partcular validation fails for a field. task is a string, if number is sent in the request body validator will throw `Task must be a string` message.

```js
const { z } = require("zod");

  z.object({
    task: z.string({
      required_error: "Task is required",
      invalid_type_error: "Task must be a string",
    }),
    isComplete: z.boolean({
      required_error: "isComplete is required",
      invalid_type_error: "isComplete must be a boolean",
    }),
  }),
```

**bcrypt**

`Installation:` `npm install bcrypt`.

`Purpose:` bcrypt helps in hashing. We should not store user passwords into database as plane strings. Its best practise to always hash the password and save. Even developers wont be able to see what the password is. We hash the password before saving to the db. We hash the password sent by the user while loggin in and compare the already hashed password saved in the db to check if the login credentials are right.

`Usage:`

```js
const bcrypt = require("bcrypt");
const salt = await bcrypt.genSalt(10); // greater the number greater security
const hashedPassword = await bcrypt.hash("password", salt);
```

Here `password` is the string we are hashing. We generate the salt and use that to hash the string `password`.

**jsonwebtoken**

`Installation:` `npm install jsonwebtoken`.

`Purpose:` Used to generate, verify and decode jwt tokens. Jwt tokens helps us to build secure systems.

`Usage:`

Creating the token:

```js
const token = jwt.sign(
  {
    id: existingUser.id,
    email: existingUser.email,
    role: existingUser.role,
  },
  "Jwt secret",
  { expiresIn: parseInt(3600) }
);
```

as 1st argument, we pass what we want to embed into the token, 2nd argument is the secret used to generate the token. This secret is requird to decode the token aswell.3rd agrument can be options. For example duration of validity of the token in seconds.

**cors**

`Installation:` `npm install cors`

`Purpose:` It is used to enable or restrict cross-origin HTTP requests in web applications. When you make an HTTP request from one domain (origin) to another domain, the browser's same-origin policy typically blocks the request for security reasons. The "cors" middleware helps you control and configure how your server responds to such requests from different origins.

`Usage:` just pass the cors as middleware to express application.

```js
const express = require("express");
const cors = require("cors");

const app = express();

// Enable CORS for all routes
app.use(cors());

// Your routes and other middleware

app.listen(3000, () => {
  console.log("Server is running on port 3000");
});
```

By adding app.use(cors()) to your Express application, you enable CORS for all routes. You can customize CORS behavior by passing options to the cors function, such as specifying allowed origins and HTTP methods.

**helmet**
`Installation:` `npm install helmet`.

`Purpose:` The "helmet" npm package is a widely used middleware for enhancing the security of web applications built with Node.js and Express.js. It provides a set of HTTP headers to help secure your application by mitigating various common security vulnerabilities. These headers are added to the HTTP responses sent by your application to protect it from threats.

Here's an overview of some key security features provided by the "helmet" package:

1. Content Security Policy (CSP): Helmet helps prevent Cross-Site Scripting (XSS) attacks by enabling you to set a Content Security Policy. CSP defines the sources from which various types of content can be loaded (scripts, styles, images, etc.), reducing the risk of malicious script execution.

2. Frameguard: Helmet includes the X-Frame-Options header to prevent your website from being embedded within an iframe on another domain, helping to mitigate Clickjacking attacks.

3. HTTP Strict Transport Security (HSTS): Helmet allows you to set the Strict-Transport-Security header, which informs browsers to always use HTTPS when connecting to your website, enhancing the security of data transmission.

4. X-Content-Type-Options: The X-Content-Type-Options header is used to prevent browsers from interpreting files as something else than declared by the server, reducing the risk of MIME type sniffing attacks.

5. X-Download-Options: Helmet sets the X-Download-Options header to prevent Internet Explorer from executing downloads in the context of your site, which can prevent certain security risks.

6. X-DNS-Prefetch-Control: This header controls DNS prefetching, which can be used to prevent browsers from automatically resolving DNS records for links on a page, reducing the risk of data leakage.

7. Referrer Policy: Helmet allows you to set the Referrer-Policy header to control how much information is included in the HTTP Referer header when navigating to external sites, improving privacy.

8. NoSniff: The X-Content-Type-Options header with the value nosniff prevents browsers from trying to guess the MIME type of a resource based on its content, reducing the risk of MIME type confusion attacks.

9. Content Security Policy (CSP) Reporting: Helmet includes options to enable CSP reporting, which allows you to collect violation reports when a policy is violated. These reports can help you identify and fix security issues.

```js
const express = require("express");
const helmet = require("helmet");

const app = express();

// Use the helmet middleware
app.use(helmet());

// Your Express routes and middleware
// ...

const port = process.env.PORT || 3000;
app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});
```

> Note: Use helmet middleware before rest of the middlewares
