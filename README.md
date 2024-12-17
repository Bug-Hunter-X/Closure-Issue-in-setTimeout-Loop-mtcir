# JavaScript Closure Issue in setTimeout Loop

This repository demonstrates a common JavaScript bug related to closures within `setTimeout` loops.  The problem arises because the closures created by `setTimeout` refer to the variable `i` by reference, not by value.  By the time the `setTimeout` callbacks finally execute, the loop has already completed, and `i` will always be its final value (10 in this case). 

**bug.js** contains the buggy code.  **bugSolution.js** provides a corrected version. 