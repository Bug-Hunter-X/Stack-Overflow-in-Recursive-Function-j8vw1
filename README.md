# Stack Overflow in Recursive Function

This repository demonstrates a common error in recursive functions: stack overflow. The `foo` function calculates the factorial of a number recursively. However, when called with a large input, it causes a stack overflow because the recursion depth exceeds the system's limits.

The `bar` function is a wrapper around `foo` that handles negative inputs gracefully.

## Bug

The bug is in the `foo` function.  The recursive calls consume stack space.  When the input is large enough, this leads to a stack overflow error.  Hack will halt execution.

## Solution

The solution involves replacing the recursive implementation with an iterative one.  This avoids unlimited stack depth.
