# PHP Loose Comparison Pitfall

This repository demonstrates a common, yet subtle, bug in PHP related to loose comparison (`==`) when comparing strings and integers. The code compares the string '0' to the integer 0 using the `==` operator.  Due to PHP's type juggling, these are considered equal, leading to unexpected behavior.

The `bug.php` file contains the erroneous code, and `bugSolution.php` offers the corrected version using strict comparison (`===`).

## How to reproduce

1. Clone this repository.
2. Run `bug.php` using a PHP interpreter.
3. Observe the unexpected output.
4. Run `bugSolution.php` to see the correct behavior.

## Learning points

- Always use strict comparison (`===`) when comparing values in PHP to avoid implicit type coercion issues.
- Be mindful of PHP's type juggling, as it can lead to unexpected outcomes if not carefully handled.