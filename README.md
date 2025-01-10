# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates an uncommon bug in HTML related to the misuse of the `innerHTML` property.  The bug occurs when attempting to set the `innerHTML` property of an element to a non-string value, such as an object literal. This will result in an error in most modern browsers.

## Bug Description

The `innerHTML` property expects a string value representing the HTML content to be inserted into the element.  Attempting to assign a non-string value (e.g., a JavaScript object) will lead to unexpected behavior or an error.

## Solution

The solution involves ensuring that the value assigned to `innerHTML` is always a string.  This can be achieved by stringifying the object or by using alternative methods for updating the DOM such as `textContent` if only text is needed.