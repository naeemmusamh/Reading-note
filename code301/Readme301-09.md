# FUNCTIONAL PROGRAMMING

What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs, that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

So how do we know if a function is pure or not? Here is a very strict definition of purity:

1. It returns the same result if given the same arguments (it is also referred as deterministic)

2. It does not cause any observable side effects

It returns the same result if given the same arguments

Imagine we want to implement a function that calculates the area of a circle. An impure function would receive radius as the parameter, and then calculate radius * radius * PI

Why is this an impure function? Simply because it uses a global object that was not passed as a parameter to the function.

Now imagine some mathematicians argue that the PI value is actually 42 and change the value of the global object.

Our impure function will now result in 10 * 10 * 42 = 4200. For the same parameter (radius = 10), we have a different result.

Now we’ll always pass the PI value as a parameter to the function. So now we are just accessing parameters passed to the function. No external object.

For the parameters radius = 10 & PI = 3.14, we will always have the same the result: 314.0

For the parameters radius = 10 & PI = 42, we will always have the same the result: 4200

# Pure functions

Pure functions are stable, consistent, and predictable. Given the same parameters, pure functions will always return the same result. We don’t need to think of situations when the same parameter has different results — because it will never happen.

# Pure functions benefits

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:

Given a parameter A → expect the function to return value B

Given a parameter C → expect the function to return value D

A simple example would be a function to receive a collection of numbers and expect it to increment each element of this collection.

let list = [1, 2, 3, 4, 5]

const incrementNumber = (list) => list.map(number => number +1);

incrementNumber(list);

For the input [1, 2, 3, 4, 5], the expected output would be [2, 3, 4, 5, 6].