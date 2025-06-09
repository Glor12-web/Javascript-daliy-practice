.

🌞 Day 14: JavaScript Forms + Form Validation
✅ What You’ll Learn
Access form values

Basic validation (e.g., not empty, correct email format)

✅ Example
html
Copy
Edit
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Day 14 - Forms</title>
</head>
<body>
    <form onsubmit="return validateForm()">
        <input type="text" id="username" placeholder="Enter your name">
        <input type="email" id="email" placeholder="Enter your email">
        <button type="submit">Submit</button>
    </form>
    <p id="error" style="color:red;"></p>

    <script>
        function validateForm() {
            let name = document.getElementById("username").value;
            let email = document.getElementById("email").value;
            let error = document.getElementById("error");

            if (name === "" || email === "") {
                error.textContent = "All fields are required!";
                return false;
            }

            if (!email.includes("@")) {
                error.textContent = "Invalid email!";
                return false;
            }

            error.textContent = "Form submitted!";
            return true;
        }
    </script>
</body>
</html>
📝 Highlights
Use .value to access form input.

onsubmit="return validateForm()" prevents form from submitting if false is returned.

You can display errors without alerts using text on the page.

