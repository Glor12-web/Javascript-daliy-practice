🚀 Ready for Day 6: Logical Operators?
🔹 Lesson Note
Logical operators are used when you want to combine multiple conditions in your if statements.

✅ Types of Logical Operators
Operator	Description	Example
&&	AND – All conditions must be true	age > 18 && isStudent == true
`		`
!	NOT – Reverses a boolean value	!isStudent (if true → false)

🔸 1. && (AND)
js
Copy
Edit
let age = 20;
let isStudent = true;

if (age >= 18 && isStudent) {
  console.log("You can apply for the scholarship.");
}
✔️ This runs only if both conditions are true.

🔸 2. || (OR)
js
Copy
Edit
let age = 17;
let hasID = true;

if (age >= 18 || hasID) {
  console.log("You can enter the event.");
}
✔️ This runs if at least one condition is true.

🔸 3. ! (NOT)
js
Copy
Edit
let isLoggedIn = false;

if (!isLoggedIn) {
  console.log("Please log in.");
}
✔️ !false becomes true, so the code runs.