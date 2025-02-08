# Uncommon HTML/JavaScript Bug: DOM Manipulation Issue

This repository demonstrates an unusual bug related to DOM manipulation in JavaScript.  The issue occurs when attempting to append a child element to a div whose `innerHTML` has just been cleared.

## Bug Description

The primary problem lies in the unexpected behavior of `appendChild` when used after setting `innerHTML` to an empty string.  The `appendChild` operation appears to succeed (no errors are thrown), but the newly appended element does not render in the browser.  This leads to an invisible DOM change.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Click the "Click Me" button.

You will observe that the div initially displays text, and that text is cleared when the button is clicked. However, the expected replacement text fails to appear, even though the DOM structure is correctly updated.

## Solution

The `bugSolution.html` file provides a corrected version of the code. 

## Contributing

Contributions are welcome!
