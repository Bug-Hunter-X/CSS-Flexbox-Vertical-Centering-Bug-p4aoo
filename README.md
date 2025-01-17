# CSS Flexbox Vertical Centering Bug
This repository demonstrates a subtle bug related to vertical centering using Flexbox in CSS.  The issue affects certain browsers where the content within a flex container doesn't center vertically when the content height is less than the viewport height.  The `bug.css` file showcases the problematic code, and `bugSolution.css` provides a solution.

**Problem:**
The standard approach of using `align-items: center;` and `justify-content: center;` with `min-height: 100vh;` on a flex container does not consistently center content across different browsers when the content height is smaller than the viewport.

**Solution:**
The solution involves adding `height: 100vh` to the container instead of using `min-height`. This guarantees the container takes up the full viewport height, ensuring proper centering.
