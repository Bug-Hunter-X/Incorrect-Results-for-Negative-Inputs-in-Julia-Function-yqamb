# Julia Function Bug: Incorrect Results for Negative Inputs

This repository demonstrates a common bug in Julia functions involving operator precedence and type instability that leads to incorrect results for negative inputs.  The bug is present in the `myfunction` function which is designed to square the input and return the squared value, changing the sign for negative numbers.  The solution demonstrates how to resolve the issue using proper operator precedence and type stability.

## Bug

The `bug.jl` file contains the buggy Julia code. The function incorrectly calculates the result when using negative numbers, due to an ambiguity in how Julia handles negative number squaring without explicit parentheses.

## Solution

The `bugSolution.jl` file contains the corrected Julia code, addressing the issues outlined in the bug section. The solution uses explicit parentheses to force the correct order of operations and ensuring type stability.
