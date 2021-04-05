# Evaluating Performance by Calculations

## Mathematical Models for Running Time
### Total Running Time
- Sum of cost x frequency for all operations.
- Need to analyse program to determine set of operations.
- Cost depends on machine, compiler

**Challenge:** How to estimate constants.

**Observation:** Most primitive operations take constant time.
**Caveat:** Non-primitive operations often take more than constant time. *E.g. abusive string concatenation.*

## Advantages/Disadvantages Over Scientific Method
### Advantages
- Precision.

### Disadvantages
- Can be tedious.
- Prone to calculation error.

**In Principle:** Accurate mathematical models are available.

**In Practice:**
- Formulas can be complicated.
- Advanced mathematics may be required.
- Exact models best left for experts.

**Bottom Line:** We use approximate models in this course.

## Cost Model 1
All constants are equal to `1`.

New generation of computers have smaller constants compared to older ones.

There are operations that do not have a constant cost. *E.g. Naive string concatenation, method calls, etc.*

## Cost Model 2
Only highest order terms count.

Estimate running time (or memory) as a function of input size `N`.
Ignore lower order terms.
- When `N` is large, terms are negligible.
- When `N` is small, we don't care.

## Cost Model 3
Simplifying the calculations. Use some basic operation as a proxy for running time.

**Careful!:** Don't over-simplify! Make sure that the operations you are not counting add up to a factor lower than the operations you do want to counting

## Combination of Cost Models
Each cost model makes a simplification in the calculation of running time. We can even combine the assumptions of different cost models.

> Performance Estimate = Simplified Number of Array Accesses
