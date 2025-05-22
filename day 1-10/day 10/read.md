✅ Day 10: Objects in JavaScript
🧠 Lesson Note
An object is a way to store key–value pairs in JavaScript.

✅ Example:

let person = {
  name: "Glory",
  age: 21,
  city: "Benin",
  isStudent: true
};

console.log(person.name);     // Glory
console.log(person['age']);   // 21
✅ How to update and add values:

person.age = 22;               // update age
person.country = "Nigeria";    // add new property
console.log(person);
✅ Object with function (method):

let user = {
  name: "Mira",
  greet: function () {
    console.log("Hi, " + this.name);
  }
};

user.greet(); // Hi, Mira
✏️ Day 10 Assignment
Create an object car with properties: brand, model, year.

Log the model to the console.

Add a new property color.

Create a method describeCar() that logs: “This is a [color] [brand] from [year].




🧠 Understanding this Keyword in JavaScript
✅ What is this?
In an object method, this refers to the object itself.

So inside your method user(), this.brand refers to car.brand.

It allows the method to access other properties of the same object.

