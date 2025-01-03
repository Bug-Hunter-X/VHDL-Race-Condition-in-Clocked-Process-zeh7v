# VHDL Race Condition Example
This repository demonstrates a common coding error in VHDL involving race conditions within clocked processes. The `bug.vhdl` file contains code exhibiting the issue, while `bugSolution.vhdl` provides a corrected version.  The problem arises from the simultaneous assignment of `data_reg` and `data_out` in the same clock cycle, which can lead to unpredictable results depending on the synthesis tool's behavior. The solution uses a more robust approach to ensure correct data flow.

## How to reproduce
1. Synthesize `bug.vhdl` with your preferred VHDL synthesizer.
2. Observe the simulation results for `data_out` to see unpredictable behavior.
3. Synthesize and simulate `bugSolution.vhdl` to see the corrected output.
