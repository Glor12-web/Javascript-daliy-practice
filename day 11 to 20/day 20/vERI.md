✅ Let's break it down step by step: 1. What is JSON? JSON (JavaScript Object Notation) is a text-based way to store and send data. Browsers don’t store real JavaScript objects, so we convert them to JSON strings with JSON.stringify(), and back into objects
with JSON.parse(). 

🧠 Code Explanation:
 ➤ Step 1: Create a JavaScript object  let user = { name: "Glory", role: "Front-End Dev", codeName: "Mira" }; You're making an object called user with 3 properties. 
 ➤ Step 2: Store the object in localStorage

(browser storage)localStorage.setItem("userData", JSON.stringify(user)); You convert the object into a JSON string using JSON.stringify(user). Then save it in localStorage with the key "userData". ✅ This means the data is saved in the browser

and stays even after the page is refreshed.


 ➤ Step 3: Retrieve it later from localStorage  let storageUser = JSON.parse(localStorage.getItem("userData")); console.log(storageUser.name); You retrieve the JSON string using localStorage.getItem("userData").
Convert it back into a JavaScript object with JSON.parse(). Then you can access any property like storageUser.name. ➤ You did the same for another object:  let lily = { name: "Lillian", role: "Backend dev" }; localStorage.setItem("userInfo",
JSON.stringify(lily)); let StoreData = JSON.parse(localStorage.getItem("userInfo")); console.log(StoreData); So now you have two different sets of user info stored separately using two keys: "userData" and "userInfo".

 ✅ Summary Table Action Code Convert
Object → JSON String JSON.stringify(object) Convert JSON String → Object JSON.parse(jsonString) Store in localStorage localStorage.setItem(key, value) Get from localStorage localStorage.getItem(key) ✅ Bonus Tip To remove data: localStorage.removeItem("userInfo");
To clear all:  localStorage.clear(); 📝 Assignment (Day 20): Create an object called profile with: username email isLoggedIn (boolean) Save it in localStorage as "profileData". Retrieve it, parse it, and display username in the console.