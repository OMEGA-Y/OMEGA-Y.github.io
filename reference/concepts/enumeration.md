## Enumeration

People should understand the concept of looping/enumerating through things.
They might not know about specific loops (`for`/`while`) or about enumerating an array using a higher-order function (like `each`), but the general concept of stepping through an array should be familiar.

Tracks should teach the normal idiomatic ways to loop/enumerate in their language, but do not need to be exhaustive about all the possibilities (e.g. don't bother teaching `for` in Ruby).

## Exercises

### Stack of cards 2

This exercise deals with analysis on a stack of playing cards. The reference implementation (JavaScript) teaches:

- Find the index of an item in an array
- Find the index of an item matching a predicate in an array
- Test a predicate against all items in an array
  - short-circuit on one true (`some`)
  - short-circuit on one false (`every`)

#### Implementations

| Track      | Exercise                              | Changes |
| ---------- | ------------------------------------- | ------- |
| JavaScript | [arrays][implementation-javascript-2] | None    |

[implementation-javascript-2]: ../../languages/javascript/exercises/concept/array-analysis/.docs/introduction.md