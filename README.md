# MongoDB $inc Operator with String Field Error

This example demonstrates an error that occurs when attempting to use the MongoDB `$inc` operator with a string field. The `$inc` operator is intended for numerical fields and will throw an error if used with strings.

The `bug.js` file contains the incorrect code, and the `bugSolution.js` file provides the corrected approach.

## How to reproduce the error

1. Create a MongoDB collection with a document containing a string field.
2. Execute the code in `bug.js`. Observe the error message.

## Solution

Use appropriate update operators for string manipulation, such as `$set` for direct replacement.  For numerical updates, ensure the target field is of a numeric type.  Refer to `bugSolution.js` for the corrected code.