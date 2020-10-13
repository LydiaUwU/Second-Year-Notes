# Relations
**Definition:** Let `A`, `B` be sets. A subset of the Cartesian product `A x B` is called a relation between `A` and `B`. A subset of the Cartesian product is `A x A` is called a relation on `A`.

Note how general this definition is. To make it useful for understanding predicates, we will need to introduce key properties relations can satisfy.

**Binary Relations:** Relations that involve 2 elements.

## Equivalence Relations
**Definition:** A relation `R` as a set of `A` is called:
- *Reflexive* if and only if for all of `x` is an element of `A`, `x` is related to `x`.
- *Symmetric* if and only if for all of `x`, `y` are elements of `a`, `x` is related to `y` implies `y` is related to `x`.
- *Transitive* if and only if for all `x`, `y`, `z` are elements of `a`, `x` is related to `y` and `y` is related to `z` implies `x` is related to `z`.

## Equivalence Relations and Partitions
**Partition:** Let `A` be a set. A *partition* of `A` is a collection of non-empty sets, any two of which are disjoint (non intersecting) such that their union is `A`.

**Definition:** If `R` is an equivalence relation on a set `A` and `x` is an element of `A`, the equivalence class of `x` is denoted as `[x]_R` is the set `{y | xRy}`. The collection of all equivalence classes is called `A` modulo `R` and denoted `A/R`.
