✅ Day 8: Loops in JavaScript
🧠 Lesson Note
Loops help you repeat actions without writing the same code again and again.

There are different kinds of loops:

1. For Loop

for (let i = 0; i < 5; i++) {
  console.log("Number:", i);
}
Explanation:

let i = 0 → Start from 0

i < 5 → Stop when i reaches 5

i++ → Increase i by 1 after each loop

2. While Loop

let count = 0;
while (count < 3) {
  console.log("Counting:", count);
  count++;
}
It continues looping as long as the condition is true.

3. Looping through an array

let fruits = ["apple", "banana", "orange"];

for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}


✏️ Day 8 Assignment
Create an array of 5 colors.

Use a for loop to print each color.

Use a while loop to print numbers from 1 to 5.


Explanation


✅ colors.length tells the loop how many times to run — it stops when all items are printed.

✅ colors[i] accesses each item based on its index.

✅ You are looping through an array, which is the most common use of for.

✅ You asked why we use a comma here:


console.log('count', i);
This is the same as:


console.log('count ' + i);
But with a comma, JavaScript adds a space automatically. So:


console.log('count', 5); // count 5
✅ This loop is just counting numbers, not looping through an array.

| **For Loop with Array**           | **Basic For Loop**                |
| --------------------------------- | --------------------------------- |
| Loops using `.length` of an array | Loops using a number as condition |
| Accesses items like `colors[i]`   | Only logs numbers like `i`        |
| Used when you have an array/list  | Used for fixed number of times    |

