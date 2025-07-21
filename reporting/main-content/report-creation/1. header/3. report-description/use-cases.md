### Positive:
* Displays the correct report description, truncated depending on the screen size.
* Supports multiline descriptions.
* Handles valid characters (including punctuation, symbols, etc.).

### Negative:
* Description missing or not shown when it exists.
* Displays raw values (“null,” “undefined”) or broken HTML if API fails or value is corrupted.
* Broken formatting with special or escape characters.
* Does not update live if the description is edited elsewhere.

### Edge:
* Very long descriptions: description overflows or breaks layout.
* Description with only whitespace, special characters, or non-Latin scripts.
* HTML or script injection attempt: verify no code executes or displays unsafely.