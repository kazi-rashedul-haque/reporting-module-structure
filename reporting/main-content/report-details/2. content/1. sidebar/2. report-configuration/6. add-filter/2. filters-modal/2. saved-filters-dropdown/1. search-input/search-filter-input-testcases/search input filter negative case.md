**Title**: Search Input Shows No Results Message

**Pre-Condition**: Filters modal is open with saved filters dropdown expanded and several saved filters available.

**Test Steps**:
    * Open the filters modal.
    * Click on the saved filters dropdown to expand it.
    * Type a search term that doesn't match any existing saved filters (e.g., "xyz123").

**Expected Result**:
    * Search input accepts the invalid search term without errors.
    * No saved filters are displayed in the results.
    * Message "No options to show" appears in the dropdown.