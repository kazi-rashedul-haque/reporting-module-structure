# TC_AddFilter_SavedFilters_010

**Title:**
Verify Saved Filters dropdown functionality for loading, searching, and managing saved filters

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. At least 3-5 saved filters exist in the system

## Test Steps:
1. Click on the "Saved Filters" dropdown button
2. Observe the dropdown interface that appears
3. Test the search functionality:
   - Type partial filter name
   - Verify filtered results
   - Clear search and verify all filters return
4. Click on a saved filter name to load it
5. Test rename functionality on a saved filter
6. Test delete functionality on a saved filter
7. Test with no saved filters available

## Expected Results:
1. "Saved Filters" button is visible with dropdown arrow
2. Clicking opens dropdown interface containing:
   - Search input field with placeholder "Search"
   - List of saved filters
   - Each saved filter has:
     - Filter name button (clickable to load)
     - Rename button (edit icon)
     - Delete button (trash icon)
3. Search functionality:
   - Search input is auto-focused when dropdown opens
   - Typing filters the list dynamically
   - Partial matches are supported
   - Case-insensitive search
   - Clear search (X button) resets to full list
   - "No options to show" message when no results
4. Loading saved filters:
   - Clicking filter name loads complete configuration
   - All conditions and nested filters are restored
   - Current filter form is replaced with saved configuration