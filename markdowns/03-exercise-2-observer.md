# Exercise 2: Observer pattern

## Goal

Use the [Observer pattern](https://refactoring.guru/design-patterns/observer) to implement a small program that complies with the specification.

Unit tests are already done for you. You should read these tests to implement carefully your program.

The exercise is considered as **complete** when all unit tests provided pass.

## Specification

A teacher wants to calculate the average note for a student.

The program must allow the teacher to add notes to a student.

Everytime the teacher add a note, the program must recalculate the average to take the new note into account.

The program obviously should be able to give the student's average when asked.

## Additional information

For this exercise, you should use the [`Observer`](https://docs.oracle.com/javase/8/docs/api/java/util/Observer.html)/[`Observable`](https://docs.oracle.com/javase/8/docs/api/java/util/Observable.html) classes of the package `java.util`.

Read the documentation carefully to leverage the Observer pattern without creating your own classes.

## Going further (optional)

`Observer` and `Observable` are [**deprecated**](https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/util/Observable.html) since Java 9.

How could you refactor your program to use the latest Java language features and best practices?
