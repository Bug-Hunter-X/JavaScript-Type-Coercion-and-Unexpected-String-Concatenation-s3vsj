# JavaScript Type Coercion Bug

This repository demonstrates a common JavaScript bug related to type coercion. The `foo` function intends to add two numbers, but due to type coercion, it performs string concatenation when one of the inputs is a string.

## Bug Description
The `+` operator in JavaScript exhibits type coercion.  When one operand is a string and the other is a number, the number is coerced into a string, and string concatenation occurs instead of numerical addition.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js`.
3. Run the code using a JavaScript runtime (e.g., Node.js).
4. Observe the unexpected output: '12' instead of 3.

## Solution
The solution involves explicit type checking and conversion to ensure numerical addition. See `bugSolution.js` for a corrected version.

## Lessons Learned
- Be mindful of JavaScript's type coercion rules.
- Always validate and convert inputs to ensure correct data types before performing arithmetic operations.
- Consider using stricter type checking (e.g., TypeScript) to prevent these kinds of errors.