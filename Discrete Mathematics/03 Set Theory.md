# Set Theory

**Set:** A collection of objects.

## Natural Numbers
ℕ the set of natural numbers starting at 0.
ℕ is defined by the following two axioms:
1. `0 ∈ ℕ`
2. if `x ∈ ℕ`, then `x + 1 ∈ ℕ (x ∈ ℕ -> x + 1 ∈ ℕ)`

## Real Numbers
ℝ is the set of real numbers, also introduced axiomatically.

> (r) **Completeness:** If a nonempty set of real numbers has an upper bound, then it has a *least* upper bound.

*There is an awful, awful lot of axioms for this so its probably best to just check the official notes for this. However the axioms for ℝ will not show up on an exam.*

## Null Set
Ø is the set with no elements. The empty set.

## The Equality of Sets
**Definition:** Let `A`, `B` be sets. `A = B` if and only if all elements of `A` are elements of `B` and all elements of `B` are elements of `A`.

## Two Ways to Describe Sets
1. **The Enumeration/Roster Method:** List all elements of the set.
2. **The Formulaic/Set Builder Method:** Give a formula that generates all elements of the set.

## Finite and Infinite
**Definition:** A set `A` is called finite if it has a finite number of elements; otherwise, it is called infinite.

## Set Operations
Connectives are integral to set operations.

**Subsets ⊆:** Let `A`, `B` be sets. `A` is a *subset* if all elements of `A` are elements of `B`.

**Proper Subsets ⊂:** Let `A`, `B` be sets. `A` is a *proper subset* of `B` if `A` is a subset of `B` and `A != B`.

**Union ⋃:** Let `A`, `B` be sets. The *union* of `A` and `B` contains all elements of both combined.

**Intersection ⋂:** Let `A`, `B` be sets. The *intersection* of `A` and `B` contains all elements that are common in both sets.

**Disjoint:** Let `A`, `B` be sets. `A` and `B` are called a *disjoint* if they share no elements. That is the intersection of the two is an empty set.

It is possible to subtract one set from another.

**Compliment:** Let `A`, `B` be sets. The *compliment* of `A` in `B` is all the elements of `B` that **are not** in `A`.

## Venn Diagrams
**Venn Diagrams:** Schematic representation of set operations.

### Pros
- Easy to visualise.

### Cons
- Misleading if sets are in some non standard configuration.
- Not helpful if a lot of sets are involved.
- Not helpful if sets are infinite or have some peculiar structure.

## Properties of Set Operations
### Commutativity
Intersection and Union are commutative.

### Associativity
Intersection and Union are associative.

### Additional Properties
- Distributivity
- De Morgan Laws
- Involutivity of the Compliment
- Transitivity of Inclusion
- Criterion for proving equality of sets.
- Criterion for probing non-equality of sets.

An involution is a map such that applying it twice gives the identity.

## The Power Set
**Definition:** Let `A` be a set. The power set of `A` denoted `P(A)` is the collection of all subsets of `A`.

`P(A)` and `A` are viewed as living as separate worlds to avoid phenomena like Russell's Paradox.

### Theorem
Let `A` be a set with `n` elements, then `P(A)` contains `2^n` elements.

### Proof
Based on the on/off switch idea.

For all elements `x` of `A`, we have two choices: either we include `x` in the subset or we don't. `A` has `n` elements implies we have `2^n` subsets of `A`.

**qed**

**Note:** It is an axiom of set theory that every set has a power set, which implies no set of all possible sets could exist, else what would its power set be?

## Cartesian Products
**Definition:** Let `A`, `B` be sets. The Cartesian product denoted by `A x B` consists of all ordered pairs `(x, y)` such that `x` is an element of `A` and `y` is an element of `B`.

## Cardinality (number of elements) in a Cartesian Product
If `A` has `m` elements and `B` has `p` elements, `A x B` has `mp` elements.

We can define Cartesian products of any length. If all sets are finite, the numbers of elements is too.
