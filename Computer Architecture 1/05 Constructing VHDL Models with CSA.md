# Constructing VHDL Models with CSA

- List all components with propagation delays.
- Identify input/output signals as input/output ports.
- All remaining signals are internal signals.
- Identify the type of each signal.
- If there are `N` signals and output ports, there will be `N` CSA statements in the VHDL model.
- CSA statements maintain a close correspondence with the hardware being modelled.
- CSA is only one out of many alternative VHDL constructs.

## Process Construct
It's difficult to simulate CSA models of large complex systems at gate level so to increase the level of abstraction whilst preserving external event behaviour we need a more powerful language construct.

### The Process Construct Allows us to:
- Model at a higher level of abstraction.
- Use conventional programming language constructs.

## Process Details
A `process` is a sequentially executed block of code, similar to conventional block structured programming languages.

- `begin` determines the start of sequential execution, and `end process` ends it.
- Programs may use standard data types and structures.
- Variable assignment occurs immediately.
- Values assigned to variables are visible to all following statements in the context of this process.
- Control flow within a process are determined by the usual constructs.
- A process can make assignments to signals declared externally.
- Propagation delay is taken into account.
- The rest of the process executes in zero time with respect to simulation.
- A process is executed if an inout signal in the list following the process has changed.
- The list of inputs is called a **sensitvity list**.
