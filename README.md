# Lua Function Nil Parameter Issue

This repository demonstrates a subtle issue with nil parameter handling in a Lua function. The `foo` function aims to add two numbers, gracefully handling cases where one or both inputs are nil. However, when both `a` and `b` are nil, it unexpectedly returns nil instead of a more sensible default value like 0.

The `bug.lua` file contains the buggy code, while `bugSolution.lua` offers a corrected version that addresses this issue.

## Problem
The original `foo` function doesn't account for the case where both parameters are nil, leading to an unexpected nil return value.