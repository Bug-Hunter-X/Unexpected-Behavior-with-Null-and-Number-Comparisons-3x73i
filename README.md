# JavaScript Type Coercion Bug

This repository demonstrates a subtle bug in JavaScript related to type coercion when comparing numbers and null values.  The `foo` function uses strict equality (`===`) to check for null values.  However, this might lead to unexpected outcomes when working with mixed types.

The bug is explained in detail in `bug.js`. A corrected version of the function is provided in `bugSolution.js`, demonstrating how to address the type coercion issue.

## Bug Details

The original function attempts to add two numbers together, returning null if either input is null.  Strict equality (`===`) is used to check for null. This can lead to issues due to JavaScript's type coercion rules. Loose equality (`==`) would provide different, and likely unexpected, results.