
We'll create a new file named index.js.
```js
console.log('hello world');

```

Run this in node using cmd by this command 
```bash
node index.js
```

You can also run this on integrated terminal on vscode. Node comes next , first we learn basics of the language.


### Variables

![Alt text](image.png)\
Boxes with labels - an analogy for the variable.

```js
// going forward from ES6 and later , we use let instead of var
let name;
console.log(name);
```

Console returns
```
undefined
```
Lets define our first variable
```js
let name = 'daksesh';
console.log(name);

// Output > daksesh
```

We cannot use reserved words as names for a variable
```js
let if = "some name";
// Throws an error 
```

Lets also have meaningful names and follow conventions , use meaningful and descriptive names.\
Also we cannot start a name with a number .\
Spaces are not allowed .\
Know about camel notation.


```js
let firstName , lastName; // for variables use camel notation
const GRAV_CONST , DEBROGLIE_CONST ; // for constants use upper case snake case
```
[For more things about casings](https://www.freecodecamp.org/news/snake-case-vs-camel-case-vs-pascal-case-vs-kebab-case-whats-the-difference/) follow the link.




### Constants
Used where we want the engine to throw an error when we try to change a constant by mistake.
```js
const INTEREST_RATE = 0.3;
INTEREST_RATE = 1;
// Throws Error 
//> TypeError: Assignment to constant variable. at index.js:3
```

### Types 
Primitive Types 
- String
- Number
- Boolean
- undefined
- null


```js
let name = 'daksesh'; // is a string literal
let number = 23; // is a number literal 
let isAgreedUpon = false; // is a boolean literal
let lastName = undefined; // 
let lastName = null; // used for explicitly clearing the value of a variable
```

null represents absense of value whereas undefined meaning the value is not assigned, for example

```js
let name;
// name has the value undefined
let name = null;
// now the name has the value null
```

### Dynamic Typing 
This is a feature that JavaScript has , that offers flexibility over the type of variable with the let keyword.
[Go the w3schools for more clarity.](https://www.w3schools.com/js/js_typeof.asp) 

```js
let name = 'daksesh'; 
let number = 23;
let isAgreedUpon = false; 
let lastName = undefined; 
let colorSelected = null; 
/*
Console
-----------------
> typeof name
< "string"
-----------------
> name = 1;
< 1
-----------------
> typeof name
< "number"
-----------------
*/

```
Above example demonstrates the dynamic typing capabilities of the JavaScript . Also note that all types of numbers are numbers in javascript unlike other languages.

```js
/* Console
-----------------
> typeof age
< "number
-----------------
> age = 30.1
< 30.1
-----------------
> typeof age
< "number"
-----------------
*/
```
Note that the 'undefined' assignment also sets the type to undefined.

```js
/* Console
-----------------
> typeof lastName
< "undefined"
-----------------
> typeof colorSelected
< "object"
*/

```
Undefined is a type and value in javascript. The last typeof is explained in the next section.




