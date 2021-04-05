# Digital System Design

```
  m""                #
mm#mm  m   m   mmm   #   m
  #    #   #  #"  "  # m"
  #    #   #  #      #"#
  #    "mm"#  "#mm"  #  "m
```

Don't think programmer, think hardware.

We want to design micro-architecture(*???????*)
Logic is defined at register control level.

Design tools are horrendously expensive.

Unlike programming you shouldn't rely on trial and error in hardware design.

The largest propagation delay in your system determines the overall speed.

## Functional Design
- Functional design is based on requirement specification.
- Target implementation influences the design flow.
- Requirements:
  -*Operation, Performance, Interface, Cost, Size, Power dissipation, ...*
- Functional design may be verified through simulation.

## Register Transfer Level Design
- This step in the design flow transforms the high-level Functional design into a description at the register level.
- The RTL desgin describes the design at the following level of abstraction:
  - Registers.
  - Memory.
  - Arithmetic Units.
  - State Machines.
- RTL designs are validated through simulation.

**HE SKIPPED THE FUCKING SLIDE IN 2 SECONDS**

## Logic Design
- At this stage in the design flow the register level transfer desgin is compiled into logic design.
- Again the design may be verified through simulation.

## Circuit Designs
= At this stage in the design flow the logic design is compiled into circuit design.
- The step is strongly influenced by the target implementation.
- Again the design may be verified through simulation specifically through:
  - Timing simulation.
  - Circuit Analysis.

## Physical Design
- In the final step in the design flow the circuit design determines the physical chip layout.
- Physical prperties may be verified by:
  - Chip Area.
  - Power dissipation.
  - Clock Frequency.

## Hardware Description Languages
- HDLs are used to:
  - Describe digital systems.
  - Model digital systems.
  - Design digital systems.
- HDLs:
  - *VHDL, verilog, ...*
