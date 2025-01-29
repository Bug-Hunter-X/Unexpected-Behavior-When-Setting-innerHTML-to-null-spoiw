# Uncommon HTML Bug: Setting innerHTML to null

This repository demonstrates an uncommon bug in HTML related to setting the `innerHTML` property of an element to `null`.  While it might seem intuitive to use `null` to clear the content of an element, some browsers handle this differently than setting it to an empty string (`""`).  This can lead to unexpected behavior or errors.

## Bug Description
The bug occurs when attempting to clear the content of a div element by setting its `innerHTML` to `null`.  In this example, the text within the div should be visible, but due to the incorrect use of `null`, it is not displayed.

## Solution
The solution is to set `innerHTML` to an empty string (`""`) instead of `null`. This consistently clears the element's content across different browsers.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Observe the unexpected behavior.  The text within the div element is not displayed.
4. Open `solution.html` in your web browser.  The text is cleared as expected.
