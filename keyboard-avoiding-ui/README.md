# Mobile Virtual Keyboard Handling Example

This page provides a simple example for **managing UI elements (especially a bottom-fixed footer) when the virtual (soft) keyboard appears on mobile web browsers**.

## Purpose

- Prevent the bottom-fixed footer from being obscured by the mobile virtual keyboard when focusing on an input field or textarea.
- Automatically adjust the position of the footer using the VisualViewport API so it always remains visible above the keyboard.

## How It Works

- Uses the **VisualViewport API** to listen for `resize` events and detect changes in viewport height caused by the virtual keyboard.
- When the keyboard appears, the footer is moved up so it stays above the keyboard.
- When the input loses focus, the footer returns to its original position.

## References

- Cross-browser mobile input UI guide (channel.io blog)
  - https://channel.io/ko/blog/articles/cross-browsing-ios15-12bccbc3
- VisualViewport API
  - https://developer.mozilla.org/en-US/docs/Web/API/VisualViewport
  - https://developer.mozilla.org/en-US/docs/Web/API/VisualViewport/resize_event
- CSS overscroll-behavior
  - https://developer.mozilla.org/en-US/docs/Web/CSS/overscroll-behavior#contain

