# Exercise 4: Bridge pattern

## Goal

Use the [Bridge pattern](https://refactoring.guru/design-patterns/bridge) to implement a small program that complies with the specification.

Unit tests are already done for you. You should read these tests to implement carefully your program.

The exercise is considered as **complete** when all unit tests provided pass.

## Specification

### Devices

A device factory produces Televisions and Radios. These are devices with common features:

- Volume
- Channel
- Enable/disable

Both types of devices store the volume information as a number between 0 and 100 (that represents the percentage of the maximum power the speakers can deliver).

There is a gotcha: whereas the radio sets the channel as a frequency (stored as a number), the television has a map of pre-programmed channels, each one assigned to a specific number (ex: 1 for "TF1", 2 for "France 2", etc).

The television cannot switch to a channel if it is not pre-programmed (present in its internal map).

You must code a program to make these devices work, respecting the factory specification and quality standards.

### Remote controls

The factory also produces two types of remote controls:

- A simple one, that performs various operations, like turning the channel up or down, turning the volume up or down, power on or off the device, and so on.
- An advanced one, which is able to mute the volume of the device.

These two types of remote controls must be able to work with all the devices produced by the factory (Television and Radio), to avoid planned obsolescence and to promote reusability of the remote controls.

You must add these features to the existing device program, without changing the device code!

## Additional information

Take a look of the [java.util.Map](https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/util/Map.html) interface and [java.util.HashMap](https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/util/HashMap.html) class.

## Going further (optional)

How to refactor this code to follow the best practices in producing quality code?
