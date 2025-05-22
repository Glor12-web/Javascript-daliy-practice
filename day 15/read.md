🌞 Day 15: Array Looping with forEach() and map()
✅ What You’ll Learn
Use forEach() to loop over arrays

Use map() to transform array data

✅ Example
html
Copy
Edit
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Day 15 - Array Methods</title>
</head>
<body>
    <h2>Check Console</h2>
    <script>
        let numbers = [1, 2, 3, 4, 5];

        numbers.forEach(function(num) {
            console.log("Number:", num);
        });

        let doubled = numbers.map(function(num) {
            return num * 2;
        });

        console.log("Doubled:", doubled);
    </script>
</body>
</html>
📝 Highlights
forEach() is used for looping but doesn't return a new array.

map() returns a new array with modified values.

Use map() when you want to transform each item.

