# Refactoring

### Functional Programming

- It is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

- The first fundamental concept we learn when we want to understand functional programming is pure functions,

#### Pure Functions characteristics:
- It returns the same result if given the same arguments.
- If our function reads external files, it’s not a pure function — the file’s contents can change.
- Any function that relies on a random number generator cannot be pure.
- It does not cause any observable side effects.


#### Referential transparency

- pure functions + immutable data = referential transparency (we can replace any expression that results in the same value and memoize it.)

