# Dart reduce() method and null values

This repository demonstrates an uncommon error that can occur when using the `reduce()` method in Dart with lists containing nullable types. The `reduce()` method is used to accumulate a single value from a list by applying a function cumulatively to each element.

The issue arises when the list contains `null` values and the function passed to `reduce()` does not handle this possibility. This will result in a runtime error.  This example showcases both the incorrect and correct approaches to handling null values during the reduction process.

## How to Reproduce

1. Clone this repository.
2. Run the `bug.dart` file. This will demonstrate the error caused by null values.
3. Run the `bugSolution.dart` file. This demonstrates a solution for handling null values.

## Solution

The solution involves checking for `null` values within the reduction function and providing appropriate default handling.  This ensures the function operates correctly regardless of the presence of `null` values within the list.