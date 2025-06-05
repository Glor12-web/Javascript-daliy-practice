✅ Day 17 – setTimeout and setInterval
Topics Covered: setTimeout, setInterval, clearInterval

💡 Explanation:
setTimeout(function, time): Runs a function once after a delay.

setInterval(function, time): Runs a function repeatedly.

clearInterval(id): Stops the interval.

✨ Example:
javascript
Copy
Edit
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