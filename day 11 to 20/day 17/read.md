✅ Day 17 – setTimeout and setInterval
Topics Covered: setTimeout, setInterval, clearInterval

💡 Explanation:
setTimeout(function, time): Runs a function once after a delay.

setInterval(function, time): Runs a function repeatedly.

clearInterval(id): Stops the interval.

✨ Example:

setTimeout(() => {
    console.log("This runs once after 2 seconds");
}, 2000);

let count = 0;
let interval = setInterval(() => {
    count++;
    console.log("Running...", count);
    if (count === 5) {
        clearInterval(interval);
    }
}, 1000);
📝 Assignment:
Create a timer that logs every second.

Stop it after 10 seconds using clearInterval().


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Countdown Color Change</title>
    
</head>
<body>

    <h1 id="countdown">5</h1>

    <script>
        let seconds = 5;
        let countdownEl = document.getElementById('countdown');

        let countdown = setInterval(() => {
            countdownEl.textContent = seconds;
            seconds--;

            if (seconds < 0) {
                clearInterval(countdown);
                countdownEl.textContent = "Changing Background...";
                document.body.style.backgroundColor = "lightblue";
            }
        }, 1000);
    </script>

</body>
</html>
