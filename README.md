# Uncommon HTML Bug: Direct div Manipulation

This repository demonstrates a subtle yet common error in HTML: attempting to directly manipulate a div element without properly selecting it via the DOM.

## The Bug
The bug lies in the JavaScript code that tries to change the innerHTML of a div.  The code uses the name "myDiv" directly, which JavaScript interprets as an attempt to use an undefined variable instead of referencing a DOM element.  This results in a runtime error.

## The Solution
The solution involves using `document.getElementById()` (or a similar DOM selection method) to retrieve the element correctly before modifying its `innerHTML`.