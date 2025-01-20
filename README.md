# Tcl String Comparison Bug: Empty String Handling

This repository demonstrates a common but easily overlooked bug in Tcl when comparing strings, specifically the improper handling of empty strings.

## The Bug
The `badproc` procedure in `bug.tcl` incorrectly compares strings without considering the possibility of empty strings. This leads to unexpected results when an empty string is passed as an argument.

## The Solution
The `bugSolution.tcl` file provides a corrected version of the procedure, explicitly checking for empty strings before performing the comparison.

## How to Reproduce
1. Clone this repository.
2. Run the `bug.tcl` script using a Tcl interpreter (e.g., `tclsh bug.tcl`). Observe the unexpected results.
3. Run the `bugSolution.tcl` script. Note that the corrected procedure now handles empty strings correctly.