# Concept
This is an idea for a "block box" program that, given an input and desired output, constructs a model/function ("the black box"),
without the user doing anything more than providing input and output.

This is essentially a symbolic execution engine, but in reverse (i.e., find the correct inputs that make a program work, not break it.

# What's The Point?
The point is to, eventually, find numerical relations and/or formulas that are unknown to the scientific world. For example, if a person put in the prime numbers from 1-100 as input, and then received the desired output as prime numbers in the range 101-200, they may receive a formula that finds a pattern to predicting prime numbers.

One may argue that by creating an implementation, one already knows the outputs one would get from putting in an input. But this is not true. There are examples of mathematical models being discovered to have multiple uses when originally only one use was thought to exist [sources needed]. For example, if a set of prime numbers was put into the model, it could be the case that it would find an implementation that returned the next prime number in the sequence -- **this would be a novel discovery.**
# A Simple Example
For example.

A programmer may type:

inputs: 2
outputs: 4

A list of functions may be returned (with names):
fun\_list = add, multiply

Where the function implementation is:

```
add(x):
	return x + 2
```

```
mult(x):
	return x * 2
```

```
square(x):
	return x ** 2
```

## Add-ons
Add-ons could easily be implemented in this idea to further specify the likelihood of getting a function that a programmer wants.

For example, perhaps a user could add more input and more test cases with expected output. This would prevent the program from returning
functions which don't yield the right inputs for all the programmer may be thinking of.

For example, in the above example, if a user really wanted square as their function to return, they may have specified:

inputs: 2, 4, 8
Output: 4, 16, 64

# Implementation

A few implementation ideas:

1) Use a list of common mathematical functions.

2) Use a list of operators to combine with operands passed into the `input` area of this program
