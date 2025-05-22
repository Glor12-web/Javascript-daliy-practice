🌞 Day 13: DOM Manipulation (Creating and Removing Elements)
✅ What You’ll Learn
How to create elements using JS

Add them to the page

Remove or replace elements

✅ Example
html
Copy
Edit
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

