# Midterm 1 Language Review

Midterm will have three parts:
1. Read a code snippet and identify parts of it (labels provided)
    - Know this review document, vocab lists at ends of chapters in *Think Python*
2. Read a problem statement and design a function to solve it (no code beyond header)
    - Review "Functions in Python", section on function design
4. Read a code listing and identify statements, local names/variables, and how they change during execution
    - Look at code examples and practice tracing the execution

## Types

What data types or data structures can we use in Python, and what attributes do they have?

Include name, a quick description, and attributes like 'immutable', 'iterable', 'sized' (i.e. has a length), 'sequence'

- int: whole number, immutable
  - `1`
- bool: yes/no true/false, immutable
  - `True`
- float: number with fractional part, immutable
  - `3.14159`
- str: text, immutable, iterable, sized, sequence
  - `'hello world'`
- list: collection of items, mutable, iterable, sized, sequence
  - `[1, 2, 3]`
- tuple: record logically connected collection of items, immutable, iterable, sized, sequence
  - `(1,)`
- dict: key-value stores, mutable, iterable, sized (not sequence!)
  - `{'a': 97, 'b': 98}`
- Callable: functions, mutable
  - `lambda x : x > 0` (lambda expression)
- Nonetype: nothing
  - `None`

## Statements

*Statements* are the "sentences" Python. What kinds of statements have we discussed?

Include a name, a quick description, and either a generic representation or simple example

- Assignment
    - *left hand side* **=** *right hand side*
    - *left hand side* should be identifier(s)
    - *right hand side* is an expression whose value is assigned to the identifier(s)
- If
  - **if** *boolean expression*:
        *statement body*
  - if the boolean expression evaluates to `True`, execute statement body
- Elif
  - **elif** *boolean expression*:
        *statement body*
  - Must follow if statement, is literally "else, if"...
- Else
  - **else**:
        *statement body*
  - Must follow some other statement, most often "if"
  - Provides "alternative execution path"
- Function Definition
  - **def** *identifier* (*parameter list*):
        *function body*
  - *parameter list* contains *positional parameters* followed by *keyword parameters*
  - *positional parameters* are matched by position in the parameter list
    - `'hello world'` in `print('hello world')` is a positional argument
  - *keyword parameters* are matched by explicitly assigning values to parameters
    - `' '` in `print('hello world', end=' ')` is a keyword argument
- While Loop
  - **while** *boolean expression*:
        *statement body*
  - Executes *statement body* as long as *boolean expression* evaluates to `True`
- For Loop
  - **for** *identifier(s)* in *iterable*:
        *statement body*
  - Executes *statement body* for each value in *iterable*, assigning that value to the *identifier* 

## Operators

Operators are frequently used in *expressions*, which are "phrases" with a value.
We sometimes refer to expressions by the *type* of value they have, and operators have certain
types with which they work. Which operators have we covered?

Include the symbol(s) used, a quick description or name, and sort by type.

### Arithmetic Operators
- `+` (addition)
- `-` (subtraction)
- `*` (multiplication)
- `**` (exponent)
- `/` (division)
- `//` (int division) truncates (or drops) the fractional portion
- `%` (modulus) returns remainder of a division

### String/Sequence Operators
- `+` (concatenate)
- `*` (repeat)
- `[]` (retrieve value)

### Boolean Operators
- `==` (logical equivalence)
- `>`, `<`, `>=`, `<=`
- `!=` (not equal to)
- *value* `in` *collection* (is *value* found in *collection*)
- `and` (logical and) short circuits
- `or` (logical or)
- `not` (logical not)
- `is` (identically equal to) `is None`

### Miscellaneous

(Anything you can remember, but can't quite place in one of the other categories)
- `.` (access member of a namespace)
  - `' '.join(some_sequence)`, `math.pi`
- `*` (tuple unpacking)


## Functions

We've introduced quite a few built-in functions. How many of them can you list and
what do they do?
- `print`
- `len`
- `min`
- `max`
- `sum`
- `abs`
- `round`
- `enumerate`
- `zip`
- `filter`
- `map`
- `sorted`
- `reversed`
- `type`
- `isinstance` (remember bools are instance of ints)
- 