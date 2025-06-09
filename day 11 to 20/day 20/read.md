✅ Day 20 – JSON & localStorage
Topics Covered: JSON.stringify(), JSON.parse(), localStorage

💡 Explanation:
localStorage: Lets you save data in the browser (even after refresh).

JSON.stringify(): Converts object → string.

JSON.parse(): Converts string → object.

✨ Example:

let user = { name: "Glory", role: "Frontend Dev" };
localStorage.setItem("userData", JSON.stringify(user));

let storedUser = JSON.parse(localStorage.getItem("userData"));
console.log(storedUser.name); // Glory
📝 Assignment:
Create an object and store it in localStorage.

Retrieve it and display it on the page.

