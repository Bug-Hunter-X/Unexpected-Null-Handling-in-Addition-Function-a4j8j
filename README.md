# Unexpected Null Handling in JavaScript Addition Function

This repository demonstrates a common JavaScript bug involving unexpected null handling within an addition function.

## Bug Description

The `foo` function adds two numbers.  However, its null handling isn't entirely robust. While it correctly returns 0 if either `a` or `b` is null, it might fail silently or produce unexpected results if other non-numeric types are passed. This could lead to subtle errors in larger applications.

## Bug Solution

The solution provides more thorough type checking and error handling using typeof operator.  It explicitly checks for numbers and throws an error if non-numeric values (excluding null) are provided.