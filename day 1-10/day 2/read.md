Just a quick tip to make your console output clearer and more readable: Add a space or some text between the two values when logging. For example:


console.log(FirstName + " " + Year);


console.log("Name: " + FirstName + ", Year: " + Year);
That way, the output in the console won’t look like one long string (like Ehigie Glory2025), but more understandable.

Also, when you tried changing the const Year, did you get an error? What did it say? If you want, you can share that too!



Awesome! Here’s Day 2: JavaScript Data Types & Basic Operations for you:

Day 2: JavaScript Data Types & Basic Operations
Lesson Note
JavaScript has different data types you’ll use all the time:

String — text, e.g. "Hello", 'Glory'

Number — numeric values, e.g. 10, 3.14

Boolean — true or false values, e.g. true, false

Null — intentional absence of value (null)

Undefined — a variable declared but not assigned yet (undefined)

Object — collections of key-value pairs (we’ll cover soon)

Array — ordered list of values (we’ll cover soon)

Basic Operations
Addition (+): for numbers or strings (concatenation)

let a = 5 + 10;          // 15
let b = "Hello " + "JS"; // "Hello JS"
Subtraction (-), Multiplication (*), Division (/) work with numbers only:

let c = 10 - 3;  // 7
let d = 4 * 2;   // 8
let e = 8 / 4;   // 2
Modulus (%) gives the remainder of division:


let f = 10 % 3;  // 1
Comparison Operators: compare values and return boolean (true/false):


5 > 3;    // true
10 === 10; // true (strict equality)
