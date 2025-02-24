# Unexpected String Concatenation in JavaScript

This example demonstrates a common error in JavaScript due to its dynamic typing. When adding a number and a string, JavaScript performs string concatenation instead of numerical addition. 

## Bug

The `foo` function intends to add two numbers. However, it incorrectly concatenates a number and a string because JavaScript does not throw an error on such implicit type coercion.

## Solution

The solution involves explicit type conversion using `parseInt()` or `Number()` to ensure both operands are numbers before addition.