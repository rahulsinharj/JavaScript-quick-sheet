# All-about-JavaScript

## Console:
  * `console.time('This code took');`
  * `console.log("Hello");`
  * `console.warn("Check this warning");` // used for warning
  * `console.log(21);`
  * `console.time('This code');`
  * `console.table({name: 'Sanya', username: 'sanya2508'});` // creates table in console
  * `console.timeEnd('This code');` // calculates processing time
  * `console.timeEnd('This code took');` // calculates processing time
  * `console.assert(20<12, '20<12 is not possible.');` // check assertion
  * `console.error('This is an error.');` // cosnole error.
  * `console.clear();` // clears console

<hr/>

## Variables:
 `var`
  `let`
  `const`
 * var declarations are globally scoped or function scoped while let and const are block scoped.
 * var variables can be updated and re-declared within its scope; let variables can be updated but not re-declared; const variables can neither be updated nor re-declared.
 * They are all hoisted to the top of their scope. But while var variables are initialized with undefined, let and const variables are not initialized.
 * While var and let can be declared without being initialized, const must be initialized during declaration.
 * The property of a const object can be change but it cannot be change to reference to the new object.
 * The values inside the const array can be change, it can add new items to const arrays but it cannot reference to a new array.

     ### Rules for creating variables:
    1. Can not start with numbers.
    2. Can start with letter, _, $.
    3. Are case sensitive.
    
     ### Most common programming case types:
    1. camelCase
    2. kebab-case
    3. snake_case
    4. PascalCase


<hr/>

## Data types:
 1. Primitive data type: (Memory allocation in stack)
    1. String
    2. Number
    3. Boolean
    4. Null (datatype is object, still primitive)
    5. undefined
    6. symbol
    
 2. Reference data type: (Memory allocation in heap; dynamic memory)
    1. Arrays
    2. Object literals
    3. Functions
    4. Dates

<hr/>

## Type conversion and coercion:
  1. String(---)
  2. Number(---)
  3. parseInt(---)
  4. parseFloat(---)
  5. .toFixed(---)

<hr/>

## String:

```
let html;
html  = "<h1> this is heading</h1>"+
        "<p> this is My para</p>";

html = html.concat('this', ' str2');
console.log(html); // <h1> this is heading</h1><p> this is My para</p>this str2
console.log(html.length); //57
console.log(html.toLowerCase()); //<h1> this is heading</h1><p> this is my para</p>this str2
console.log(html.toUpperCase()); //<H1> THIS IS HEADING</H1><P> THIS IS MY PARA</P>THIS STR2

console.log(html[1]); //h
console.log(html.indexOf('<')); //0
console.log(html.lastIndexOf('<')); //44
console.log(html.charAt(3)); //>
console.log(html.endsWith('dsfsdfd')); //false
console.log(html.includes(' fg')); //false
console.log(html.substring(1,6)); //h1> t
console.log(html.slice(0, 4)); // <h1>
console.log(html.split('>')); // (5) ["<h1", " this is heading</h1", "<p", " this is My para</p", "this str2"]
console.log(html.replace('this', 'it')); // <h1> it is heading</h1><p> this is My para</p>this str2
```

<hr/>

## Arrays and objects:

```
let marks = [34, 23, 24, 93 ,73, 25];
const fruits = ['Orange', 'Apple', 'Pineapple'];
const mixed = ['str', 89, [3, 5]];

const arr = new Array(23,123,21, 'Orange');
console.log(marks);
console.log(mixed);
console.log(fruits[1]);

let value = marks.indexOf(73);
console.log(value)

// Mutating or Modifying arrays
marks.push(3564); // push in array
marks.unshift(1009); // push front
marks.pop(); // pop
marks.shift(); // pop front
marks.splice(2, 3); remove elements from 2nd position, and total number of elemets removed is 3.
marks.reverse(); // reverse
let marks2 = [1, 2,3, 7]
marks = marks.concat(marks2); // concat in array


let myobj = {
    'name': 'sanya', 
    isActive: true,
    username: 'sanya2508'
}

console.log(myobj)
console.log(myobj['name'])
console.log(myobj.name)
           
```

!=, == // compares value.
!==, === // compares type and value both.


// if else switch
// loops 
// function
