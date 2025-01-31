# CSS Specificity Bug: Unexpected Color Inheritance

This repository demonstrates a subtle bug related to CSS specificity and inheritance. The unexpected inheritance behavior can lead to unpredictable styling across different browsers.

## Bug Description

A paragraph element nested within a div element doesn't inherit the expected color due to specificity issues. The paragraph inherits the color declared for the `p` selector rather than the `div p` selector, despite the intent to override it. This inconsistency highlights potential issues with the cascade order and how CSS specificity interacts with inherited styles.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` to see the problematic CSS code.
3. Create an HTML file with a div containing a paragraph. 
4. Link the `bug.css` stylesheet to the HTML file.
5. Observe the paragraph's color. It might not be green as expected.

## Solution

The `bugSolution.css` file shows a fix by increasing the specificity of the overriding style, ensuring it takes precedence.