✅ Day 16 – Advanced DOM Manipulation
Topics Covered: createElement, appendChild, removeChild, dynamic DOM changes

💡 Explanation:
createElement(): Creates a new HTML element.

appendChild(): Adds an element to the DOM.

removeChild(): Removes an element from the DOM.

✨ Example:
javascript
Copy
Edit
let ul = document.createElement('ul');
document.body.appendChild(ul);

let li = document.createElement('li');
li.textContent = 'Learn JavaScript';
ul.appendChild(li);

// Remove it after 3 seconds
setTimeout(() => {
    ul.removeChild(li);
}, 3000);
📝 Assignment:
Create a list.

Add a button to dynamically add a list item.

Add a "Remove Last Item" button.

