# Uncommon CSS Flexbox Centering Bug
This repository demonstrates a subtle bug related to CSS flexbox centering and percentage heights.  The issue arises when attempting to center a box that uses percentage-based height within a flex container.

## Problem
The `bug.css` file contains CSS that intends to center a box within its parent container using flexbox. However, due to the interaction between percentage heights and flexbox, the centering may fail if the container's height isn't explicitly set.

## Solution
The `bugSolution.css` file provides the corrected CSS that addresses this issue. The key fix is to provide an explicit height (e.g., `height: 100vh;`) to the container element.  This ensures the flex container has a defined height which is then used to calculate and enforce the percentage heights of its children. 