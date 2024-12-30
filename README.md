# Unexpected Immutability of Class Attribute in Ruby

This repository demonstrates a common error in Ruby where developers unintentionally create immutable attributes within a class due to the absence of a setter method.

The `bug.rb` file showcases the problem: An attempt to change the value of an instance variable fails because no setter method is defined. The `bugSolution.rb` file provides the corrected version.  This example highlights the importance of clearly defining accessor methods (getters and setters) for instance variables to control mutability.

## How to reproduce the bug:
1. Clone this repository.
2. Run `bug.rb`.
3. Observe that attempting to change the value of `@value` has no effect.

## Solution:
Examine `bugSolution.rb` for the corrected code, which includes a `value=` method to allow modification of the instance variable.