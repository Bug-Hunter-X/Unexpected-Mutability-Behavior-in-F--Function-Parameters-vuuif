# F# Mutable Variable Swap Bug

This example demonstrates a common pitfall when working with mutable variables in F# functions.  The intention is to swap the values of `x` and `y`, but the original variables remain unchanged.

The `bug.fs` file shows the problematic code. The `bugSolution.fs` file shows a corrected version.  The issue is that the function receives copies of the variables' values rather than references.