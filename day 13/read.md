🌞 Day 13: DOM Manipulation (Creating and Removing Elements)
✅ What You’ll Learn
How to create elements using JS

Add them to the page

Remove or replace elements

✅ Example

<!DOCTYPE html>
<html lang="en">
<head>
    <title>Day 13 - DOM</title>
</head>
<body>
    <button onclick="addItem()">Add Item</button>
    <button onclick="removeItem()">Remove Item</button>
    <ul id="list"></ul>

    <script>
        function addItem() {
            let list = document.getElementById("list");
            let newItem = document.createElement("li");
            newItem.textContent = "New List Item";
            list.appendChild(newItem);
        }

        function removeItem() {
            let list = document.getElementById("list");
            if (list.lastChild) {
                list.removeChild(list.lastChild);
            }
        }
    </script>
</body>
</html>
📝 Highlights
document.createElement() creates new elements.

appendChild() adds it to the page.

removeChild() removes a specific child element.

Always check if a child exists before trying to remove it.

Day 13 – Create a Simple To-Do List
Topics Covered: DOM creation, event handling, arrays

Assignment:

Create an input field and a button.

When the button is clicked:

Add the input value to an array.

Display the updated list in the browser using JavaScript.

Bonus: Add a "Clear" button to reset the list.


✅ Day 13 – Grocery List App (Similar to To-Do List)
Topics Covered:

DOM manipulation

Arrays

Event handling

createElement, appendChild, .value

🛒 What You’ll Build:
An input field to type a grocery item.

An “Add Item” button to store items in an array and display them.

A “Clear List” button to reset everything.

