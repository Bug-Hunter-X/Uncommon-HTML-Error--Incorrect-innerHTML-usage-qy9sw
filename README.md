# Uncommon HTML Error: Incorrect innerHTML usage

This repository demonstrates an uncommon error that can occur when using the `innerHTML` property in JavaScript within an HTML context.  The error arises from attempting to assign a non-string value (specifically a number) to `innerHTML`, which can lead to unexpected behavior or silent failures.

## Bug Description
The bug lies in the incorrect usage of `innerHTML`.  The `innerHTML` property expects a string value to represent the HTML content to be inserted.  Assigning a number directly, as shown in the `bug.html` file, can result in unexpected behavior or an error in some browsers.

## Solution
The solution is simple: ensure that the value assigned to `innerHTML` is always a string. This can be achieved by converting the non-string value (like a number) to a string using the `toString()` method before assignment.

## How to reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the unexpected behavior (the number might not be displayed correctly or might cause an error).
4. Open `bugSolution.html` to see the corrected code.
