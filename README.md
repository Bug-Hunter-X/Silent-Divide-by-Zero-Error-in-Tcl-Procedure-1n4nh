# Silent Divide-by-Zero in Tcl

This repository demonstrates a subtle bug in Tcl: a divide-by-zero error that occurs silently within a procedure if not properly handled.  The `bug.tcl` file contains the flawed code, and `bugSolution.tcl` provides a corrected version.

The issue arises from the lack of error handling when the input variable 'a' is zero. The original code does not check this condition before the division occurs, leading to a runtime error that, without proper error handling, is simply ignored. The improved version provides a more robust solution by handling the exceptional case explicitly.