### Positive:
* Displays the correct report name as saved/created by the user.
* Handles all valid characters and formatting (capitalization, symbols if allowed).
* Correct truncation or wrapping if report name is too long for header width.

### Negative:
* Shows broken formatting with special characters (e.g., HTML, emoji, scripts).
* Report name is not updated after renaming it elsewhere.

### Edge:
* Very long report names: name overflows, breaks layout, or causes horizontal scroll.
* Report name with only whitespace, special characters, or non-Latin text.