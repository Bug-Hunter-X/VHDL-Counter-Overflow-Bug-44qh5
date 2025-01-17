# VHDL Counter Overflow Bug

This repository demonstrates a subtle bug related to integer overflow in a simple VHDL counter.  The provided `bug.vhdl` file contains a counter that increments on each rising clock edge. However, it lacks proper handling for the case when the counter reaches its maximum value (15).  This can lead to unexpected behavior and potentially introduce errors in a larger design.

The solution, located in `bugSolution.vhdl`, addresses the overflow issue by using a `mod` operator to ensure that the counter wraps around correctly.