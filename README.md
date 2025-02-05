# CSS calc() Unexpected Behavior with Undefined Parent Width

This repository demonstrates an uncommon CSS bug involving the `calc()` function and its interaction with percentage values when the parent element's width is undefined or not explicitly set.

The `bug.css` file shows the problematic code, while `bugSolution.css` provides a solution.

## Problem

Using `calc(100% - 10px)` on an element with a parent that doesn't have a defined width leads to unreliable results.  The calculation relies on the parent's width, which is undefined, leading to unexpected rendering or overflow.

## Solution

Ensure the parent element has a defined width (e.g., using `width: 100%;` or a fixed pixel value). This provides a reliable base for the `calc()` function to work correctly.