# Formal Languages

**Word:** For all of `n` is an element of `N*`, we define a word of length `n` in the alphabet `A` as being any string of the form `a_1, a_2, ... a_n` such that `a_i` is an element of `A`. Let `A^n` be the set of all words of length `n` over the alphabet `A`.


**Language:** Let `A` be a finite set. A *language* over `A` is a subset of `A*`.

**Formal Language:** A language `L` over `A` is called a *formal language* if there exists a finite set of rules or algorithm that generates exactly `L`.

**Grammar:** A (formal) grammar is a set of production rules for strings in a language. To generate a language we use:
1. The set `A`, which is the alphabet of the language.
2. A start symbol `<s>`.
3. A set of production rules.
