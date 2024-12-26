# F# Mutable Variable Bug

This repository demonstrates a common error in F# related to mutable variables and their interaction with function calls. The `bug.fs` file contains code that shows an unexpected result due to the way mutable variables are handled. The `bugSolution.fs` file presents a revised version, fixing the issue.

## How to reproduce

1. Clone this repository.
2. Open `bug.fs` in an F# editor or compiler.
3. Run the code. Observe the output.
4. Compare the output to the intended behavior as explained in the description.

## Solution

The solution involves understanding that once a mutable variable's value is used in a function calculation, the calculation is done using that specific value at the time of calculation. Subsequent changes to the variable won't affect the previous result.