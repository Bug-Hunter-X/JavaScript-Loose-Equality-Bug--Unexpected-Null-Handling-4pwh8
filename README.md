# JavaScript Loose Equality Bug: Unexpected Null Handling

This repository demonstrates a common JavaScript bug related to loose equality (==) and null value handling.  The `bug.js` file contains code that uses loose equality to check for null values. This can lead to unexpected behavior because loose equality does not always reliably distinguish between null and other values like 0 or an empty string. The `bugSolution.js` demonstrates using strict equality (===) to fix the issue. 

## Problem

The original code uses loose equality (`==`) to check for null values. Loose equality performs type coercion, which can lead to unexpected results when comparing values of different types. 

## Solution

The solution uses strict equality (`===`) to prevent type coercion. Strict equality only returns true if both values are of the same type and have the same value.  This eliminates the potential for unexpected results when dealing with null values. Using strict equality ensures that the function behaves as expected, correctly handling null values and producing the correct sum for non-null inputs.