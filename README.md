# Julia Bug: Unexpected Behavior with Exponentiation and Negative Numbers

This repository demonstrates a potential bug in Julia code involving exponentiation and the handling of negative numbers.  The issue arises from type instability and the behavior of the `^` operator. The `bug.jl` file contains the erroneous code.  `bugSolution.jl` offers a corrected version.

## Bug Description

The original code utilizes `x^2` to calculate the square of a number.  However, this operation can produce unexpected results when `x` is a negative number depending on the input type.  This can lead to incorrect calculations or type errors.

## Solution

The solution involves using the `abs()` function to ensure the input to `^` is always non-negative, thereby preventing the unexpected behavior. This avoids potential type instability issues.