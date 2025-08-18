**Title:** Verify Search Input functionality in Saved Filters dropdown filters results correctly

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Multiple saved filters exist (at least 5 filters with different names)
5. Saved Filters dropdown is expanded

## Test Steps:
1. Locate the search input field in the Saved Filters dropdown
2. Verify the search input displays placeholder text "Search"
3. Click in the search input field and verify it gets focus automatically
4. Type a partial search term that matches some filters (e.g., "Customer")
5. Observe the filtered results in real-time
6. Clear the search term and verify all filters are shown again
7. Type a search term that returns no results (e.g., "xyz123")
8. Verify the no results message appears
9. Test the clear button (X) functionality
10. Test with special characters and very long search terms

## Expected Results:
1. Placeholder text "Search" is displayed when field is empty
2. Input field automatically receives focus when dropdown opens
3. Real-time filtering works as user types:
   - Matching filters are displayed
   - Non-matching filters are hidden
   - Partial matches work correctly (e.g., "fil" matches "My Filter")
4. Clearing search term restores all available filters
5. When no filters match search term:
   - Message "No options to show" is displayed
6. Clear button (X) functionality:
   - Button appears when text is entered
   - Clicking X clears the search and shows all filters
7. Input handles special characters gracefully without breaking UI
8. Very long search terms don't cause layout overflow