# F# Mutable Variable Swap Bug

This repository demonstrates a common misunderstanding of how mutable variables behave in F# when used in functions.  In imperative languages like C++ or Java, the following code would correctly swap two variables. In F#, it will not work as expected. This example shows the unexpected behavior and provides a corrected solution.

## Bug
The `swap` function attempts to swap two mutable variables, but due to the way F# handles variable scope, it doesn't correctly swap the original values. 

## Solution
The solution shows the use of tuples to correctly swap variables.