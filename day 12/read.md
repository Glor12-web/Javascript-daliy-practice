🌞 Day 12: JavaScript Events (Click, Mouseover, etc.)
✅ What You’ll Learn
What are Events in JavaScript?

Common event types (click, mouseover, mouseout, dblclick, etc.)

addEventListener() vs inline event

🧠 Key Concepts
An event is an action that occurs in the browser, like clicking a button, hovering over text, or typing into an input field. JavaScript allows you to respond to these events.

✅ Example
html
Copy
Edit
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Day 12 - Events</title>
</head>
<body>
    <h2 id="text">Hover or Click me!</h2>
    <button onclick="changeText()">Click</button>

    <script>
        let heading = document.getElementById("text");

        heading.addEventListener("mouseover", function () {
            heading.style.color = "blue";
        });

        heading.addEventListener("mouseout", function () {
            heading.style.color = "black";
        });

        function changeText() {
            heading.textContent = "Button Clicked!";
        }
    </script>
</body>
</html>
📝 Highlights
mouseover and mouseout handle when you hover on or off an element.

addEventListener() gives better control than inline events (onclick="...") because you can add multiple handlers.

