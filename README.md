# CSS :focus-visible Issue with Custom Checkboxes

This repository demonstrates a bug related to the `:focus-visible` pseudo-class and custom styled checkboxes.  The checkbox appears visually unchecked after clicking, even when programmatically checked. This is observed when the checkbox receives initial focus.

## Bug Description
The problem occurs when combining custom checkbox styling with the `:focus-visible` pseudo-class.  After clicking the checkbox (and it is correctly checked programmatically), the visual representation may remain unchecked. This is especially evident when the checkbox is initially focused.

## Steps to Reproduce
1. Clone the repository.
2. Open `index.html` in a web browser.
3. Click the checkbox. Note the visual appearance.
4. Observe the behavior when the checkbox is first focused.

## Solution
The solution involves careful consideration of the order and specificity of CSS rules, potentially adding additional selectors to address the focus state explicitly.  See the `bugSolution.css` file for a possible fix. 