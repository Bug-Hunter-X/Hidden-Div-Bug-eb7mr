# Uncommon HTML Bug: Incorrect getElementsByTagName Usage

This repository demonstrates a subtle bug related to the use of `getElementsByTagName` in HTML/JavaScript.  The code intends to hide a div element on page load, but due to an incorrect understanding of `getElementsByTagName`'s return value, it may fail or cause unexpected behavior. 

The `bug.html` file shows the incorrect code, while `bugSolution.html` shows the corrected implementation.

## Bug Description

The function `getElementsByTagName` returns a NodeList, not a single element.  Attempting to directly manipulate its style without selecting a specific index can lead to errors.

## Solution

The solution uses `getElementById` to directly access the element by its ID, providing a clearer and more reliable way to manipulate the element's style. 