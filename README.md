# Uncommon JavaScript Bug: Implicit Null Handling

This repository demonstrates a common yet often overlooked error in JavaScript: implicit handling of null values.  Many developers assume loose comparison (==) will catch nulls, but that's not always true and can lead to unexpected results. This example shows how to proactively handle nulls to create robust functions.

## The Bug

The `bug.js` file contains a function `foo` that adds two numbers.  However, it doesn't explicitly handle cases where one or both inputs are `null`. This can lead to silent failures or unexpected behavior depending on the context.

## The Solution

The `bugSolution.js` file fixes this by explicitly checking for `null` values and returning `null` in those cases.  This makes the function's behavior predictable and prevents potential issues.