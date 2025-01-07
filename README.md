# Tcl == Operator Pitfall
This repository demonstrates a subtle but common error when using the `==` operator for numerical comparison in Tcl.  The `==` operator performs a string comparison, not a numerical one if the operands are strings. This can lead to unexpected results. The provided `bug.tcl` shows an example and `bugSolution.tcl` offers a corrected version using the `expr` command.

## How to reproduce
1.  Clone the repository
2.  Run `tclsh bug.tcl`
3.  Observe the unexpected output.
4.  Run `tclsh bugSolution.tcl`
5.  Observe the corrected output.