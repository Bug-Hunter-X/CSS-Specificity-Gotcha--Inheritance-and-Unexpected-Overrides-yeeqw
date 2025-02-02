# CSS Specificity Gotcha: Inheritance and Unexpected Overrides

This repository demonstrates a subtle but important CSS specificity issue related to inheritance and how it interacts with more specific selectors.  The bug showcases how a seemingly simple CSS rule can behave unexpectedly due to the intricacies of CSS specificity calculations.

## Bug Description

The core problem lies in understanding how CSS specificity works when dealing with inherited styles.  A selector with higher specificity will always override a selector with lower specificity, even if the lower specificity selector is inherited.

## How to Reproduce

1. Open `bug.css`.
2. Observe the unexpected color of the paragraph element inside the div in your browser. It isn't what a developer might expect due to a misunderstanding of how specificity and inheritance interact.

## Solution

The solution (`bugSolution.css`) demonstrates a correct way to achieve the desired effect by adjusting selectors or using the `!important` flag (with caution) to force specific styles.