# Exercise 3: Factory Method pattern

## Goal

Use the [Factory Method pattern](https://refactoring.guru/design-patterns/factory-method) to implement a small program that complies with the specification.

Unit tests are already done for you. You should read these tests to implement carefully your program.

The exercise is considered as **complete** when all unit tests provided pass.

## Specification

A huge fan of geometry wants to calculate automatically the area of some shapes:

- A circle
- An equilateral triangle
- A square

You should develop a factory that will allow the geometry fan to instantiate the right shape given the following criterion:

- Number of sides
- Side length

The instantiated shape must give the correct perimeter and area given the side length.

## Additional information

Here are the formulas for common shapes in geometry:

|        Shapes        |  Perimeter  |            Area            |
|----------------------|-------------|----------------------------|
| Circle               | $`2 \pi r`$ | $`\pi r^2`$                |
| Equilateral triangle | $`3 a`$     | $`\frac{\sqrt{3}}{4} a^2`$ |
| Square               | $`4 a`$     | $`a^2`$                    |

Notes:

- $`a`$ is the side length
- $`r`$ is the radius of a circle
- A circle only has one side, and the length of its side is actually equivalent to the circle's perimeter. But the geometry fan wants the Circle class to store the **radius** of the circle, and not the perimeter directly.
- There **cannot** be a shape with two sides.

Take a look of the [java.lang.Math](https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/lang/Math.html) class: there are methods that help to calculate these formulas.

## Going further (optional)

- Add a new shape (for example, an [hexagon](https://www.youtube.com/watch?v=thOifuHs6eY)).
- Add a new formula (ex: the volume for 3-dimensional shapes like a cube).

Obviously, you must refactor your code and unit tests to take into account the new features.
