# Concurrent Signal Assignments Statements

Digital systems operate with concurrent signals.

VHDL uses *signal assignment* statements. Multiple of these statements are executed concurrently.

### VHDL Must Specify
- Events
- Delays
- Concurrency

## CSA Statements

```vhdl
architecture concurrent_behavior of half_adder is
begin
  sum <= (x or y) after 5 ns;
  carry <= (x and y) after 5 ns;
end concurrent_behavior;
```

- `concurrent_behaviour` is the name of the architecture that defines the endtiy.
- *Signal assignment* statements:
  - `sum <= (x or y) after 5 ns;`
  - `carry <= (x and y) after 5 ns;`

## After Keyword
- Signal propagation of the XOR and AND gates must be taken into account.
- *Signal assignment* statments define this through the `after` keyword.
- This keyword specifies when the output signal is set to the result of an evaluation after an event.
- The textual order of the assignment has no influence on the timing.

## Library and Use Clauses
- A `library` contains premade entities that can be used.

## The Full-Adder Model
- The full-adder simulates the signal transitions at a gate-level.
- The model has three internal signals, these signals are not ports to the entity.
- The internal signals are declared in the architectural declaration.
- The Boolean equations define how each signal is derived as a function of:
  - Other signals.
  - Propagation delay.
- `constant` can be used to declare a constant of a particular type. In this case `Time`.

## Signals and Time
- Signals are not variables, they have a history of values over time/waveform.
- Signals may use the assignment symbol ``:=``.
- If signals aren't initialised they will receive a default value.

## Multiple Signal Transactions
It is possible to specify the following:

```vhdl
s1 <= (x xor y) after 5 ns, (x or y) after 10 ns, (not x) after 10 ns;
```

- After one of the signals changed all three waveform elements will be evaluated and scheduled according to their specification.
- The simulation keeps an ordered list of all transactions scheduled for a particular signal.
- Also known as **Projected Output Waveform**.

## Resolved Signals
- In a physical system a wire (signal) has a driver, this driver determines the waveform.
- VHDL determines the value of the signal with multiple drivers through a resolution function.
- A shared signal must be declared as a resolved type.
