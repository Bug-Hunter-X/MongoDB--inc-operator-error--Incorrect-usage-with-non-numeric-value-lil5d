# MongoDB $inc operator error: Incorrect usage with non-numeric value
This repository demonstrates an example of an error that can occur when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment or decrement a numeric field in a document.  Attempting to use it with a non-numeric value will result in an error.

## Bug
The `bug.js` file contains code that incorrectly uses the `$inc` operator.  It attempts to increment a field with a string value. This will throw an error because the `$inc` operator only works with numeric values. 

## Solution
The `bugSolution.js` file shows the corrected code.  It ensures that only numeric values are incremented using the `$inc` operator. 