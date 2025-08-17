**Title**: Search Input Successfully Filters Saved Filters

**Pre-Condition**:
1.  Multiple saved filters available.

**Test Steps**:
1. Login to the workspace as an authenticated user.
2. Navigate to the report details page.
3. Open the filters modal by clicking the "Add Filter" button.
4. Click on the saved filters dropdown to expand it.
2. Click on the saved filters dropdown to expand it.
3. Click in the search input field.
4. Type a partial filter name (e.g., "My" to find "My Filter").

**Expected Result**:
    * Search input field is focused and accepts user input.
    * Saved filters list dynamically updates to show only matching results.
    * Matching filters are displayed based on the search term.
    * Search is case-insensitive and works with partial matches.