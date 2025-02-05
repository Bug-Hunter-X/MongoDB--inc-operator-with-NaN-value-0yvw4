# MongoDB $inc operator with NaN value
This example demonstrates an incorrect usage of the `$inc` operator in a MongoDB update query.  The `$inc` operator is used to increment a numerical field, but attempting to increment by `NaN` (Not a Number) will result in an error.

## Bug
The bug lies in using `NaN` as the increment value in the `$inc` operator. This leads to an error because `NaN` cannot be added to a number.

## Solution
The solution is to ensure that the increment value is a valid number.