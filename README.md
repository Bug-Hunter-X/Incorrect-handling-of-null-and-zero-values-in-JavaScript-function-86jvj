# Incorrect Handling of Null and Zero Values in JavaScript Function

This repository demonstrates a common error in JavaScript function handling where null and zero values are treated as equivalent, leading to incorrect results.  The original function fails to distinguish between an intended null value and a numeric 0.

## Bug Description

The JavaScript function `foo` incorrectly handles null and zero values. If either input (`a` or `b`) is null, the function immediately returns null, regardless of the value of the other input. This results in incorrect output when one input is 0.

## Solution

The solution uses stricter comparison to treat 0 and null separately, allowing the function to return the correct values in all situations, including those where one or both inputs are 0. 
