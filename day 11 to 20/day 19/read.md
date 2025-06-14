✅ Day 19 – Array Methods: map, filter, find
Topics Covered: map(), filter(), find()

💡 Explanation:
map(): Transforms each item in the array.

filter(): Returns only items that meet a condition.

find(): Returns the first item that matches.

✨ Example:

let numbers = [1, 2, 3, 4, 5];

let doubled = numbers.map(n => n * 2); // [2, 4, 6, 8, 10]
let evens = numbers.filter(n => n % 2 === 0); // [2, 4]
let firstEven = numbers.find(n => n % 2 === 0); // 2
📝 Assignment:
Create an array of numbers.

Use map to double them.

Use filter to return numbers greater than 5.

Use find to get the first number greater than 5.

Method	What it Does	Example Result
.map()	Transforms each element in an array	[2, 4, 6, ...]
.filter()	Filters elements based on a condition	[6, 7, 8]
.find()	Finds the first element that matches a condition	6

📝 Optional Assignment (Day 19):
Create your own array of names:

js
Copy
Edit
let names = ["Glory", "Ada", "John", "Daniel", "Grace"];
Use .filter() to get only names longer than 4 characters.

Use .map() to convert all names to uppercase.

Use .find() to find the first name that starts with "G".