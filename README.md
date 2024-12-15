# MongoDB $inc operator error
This example demonstrates an uncommon error that can occur when using the `$inc` operator in MongoDB. The error arises from providing a string value instead of a numeric value for the increment.

## Problem
The code attempts to increment the `counter` field in a document by 1. However, it uses the string '1' instead of the integer 1. This results in an error, as `$inc` expects a numeric value.

## Solution
The solution involves ensuring that the value passed to the `$inc` operator is a number (integer or double). This corrects the operation and increments the field correctly.