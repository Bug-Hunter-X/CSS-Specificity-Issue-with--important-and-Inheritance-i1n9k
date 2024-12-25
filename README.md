# CSS Specificity Bug

This repository demonstrates a subtle bug related to CSS specificity and inheritance when using the `!important` flag.  The bug occurs because the `!important` declaration on a parent element affects its children, even if a more specific selector is applied to the child.

## Bug Description

The `bug.css` file contains CSS code where a parent element sets a `font-size` with `!important`.  A child element attempts to override this with a more specific selector and a different `font-size`. The `!important` declaration prevents this override, leading to unexpected results.

## Solution

The `bugSolution.css` file demonstrates a solution that avoids the use of `!important` in this case, solving the specificity conflict.

This repository is intended to illustrate an uncommon situation in CSS and highlight a potential pitfall to avoid.  Avoid relying on `!important` unless strictly necessary, as it can create issues with maintainability and unexpected behavior.