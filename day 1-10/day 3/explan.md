✅ Day 3: JavaScript let, const, and var + Scope
Lesson Note
There are three main ways to declare variables in JS:

1. let
Can be updated but not re-declared in the same block.

Block-scoped (works only within the {} it's defined in).


let age = 25;
age = 26; // ✅ OK
2. const
Cannot be updated or re-declared.

Must be assigned a value when declared.


const name = "Glory";
// name = "Ehigie"; ❌ Error
3. var
Function-scoped, not block-scoped.

Can be updated and re-declared.


var country = "Nigeria";
var country = "Ghana"; // ✅ Works, but not recommended
✅ Scope Example:

{
  let a = 10;
  const b = 20;
  var c = 30;
}
// console.log(a); ❌ Error
// console.log(b); ❌ Error
console.log(c); // ✅ Works

✅ Day 3: JavaScript let, const, and var + Scope
In JavaScript, we use let, const, and var to create variables. But they behave a little differently.

🔹 1. let — Modern, Safe, Block Scoped
You can change the value later.

But you cannot re-declare it in the same block.

It only works inside the block {} where it’s declared.


let name = "Glory";
name = "Ehigie"; // ✅ You can change it

let name = "Another"; // ❌ ERROR: You can't re-declare it in the same block
🔹 2. const — Constant (Cannot Change)
You must assign a value when creating it.

You cannot change the value.

You cannot re-declare it.

It's also block-scoped.


const year = 2025;
// year = 2030; // ❌ ERROR: Cannot change
🔹 3. var — Older Way (Avoid if possible)
You can change the value.

You can re-declare it (not good practice).

It is function-scoped — not block-scoped (it leaks outside {}).


var city = "Benin";
var city = "Lagos"; // ✅ Works (but confusing)
🔍 Understanding Scope
Scope means where the variable can be used (inside or outside the block {}).

Example:

{
  let a = 10;
  const b = 20;
  var c = 30;
}

console.log(a); // ❌ ERROR (a is not visible outside the block)
console.log(b); // ❌ ERROR
console.log(c); // ✅ This works because var is not block-scoped
✅ Summary
Feature	let	const	var
Can update?	✅ Yes	❌ No	✅ Yes
Can re-declare?	❌ No	❌ No	✅ Yes
Scope	Block	Block	Function (global-ish)







