# TC_AddFilter_DeleteFilterModal_020

## Title:
Verify Delete Filter modal confirms deletion and removes saved filter permanently

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. At least one saved filter exists (e.g., "Customer Experience Filter")
5. Saved Filters dropdown is expanded showing filter list

## Test Steps:
1. Locate a saved filter with delete button in the filter list
2. Click the "Delete Filter" button (trash icon)
3. Verify Delete Filter confirmation modal opens
4. Examine all modal elements and content
5. Test the Close button (×) functionality
6. Reopen delete modal and test Cancel button functionality
7. Reopen delete modal and test Delete button functionality
8. Verify filter is removed from saved filters list
9. Test deleting the last remaining saved filter
10. Test deleting multiple filters sequentially
11. Test accessibility features of the modal

## Expected Results:
1. Delete Filter modal opens successfully when delete button is clicked
2. Modal displays correct elements:
   - Modal title: "Delete Filter"
   - Confirmation message: "Are you sure you want to delete '<Filter Name>'?"
   - Filter name is dynamically populated in the message
   - Close button (×) in top-right corner
   - Cancel button (secondary/gray styling)
   - Delete button (red/danger styling)
3. Close button (×) functionality:
   - Clicking closes modal without deleting filter
   - Filter remains in saved filters list
   - Returns to Filters modal
   - No confirmation or warning messages
4. Cancel button functionality:
   - Clicking closes modal without deleting filter
   - Filter remains in saved filters list
   - Returns to Filters modal
   - Consistent behavior with Close button
5. Delete button functionality:
   - Clicking permanently removes the selected filter
   - Modal closes immediately after deletion
   - Filter is removed from saved filters list
   - Deletion cannot be undone
   - Success feedback may be provided
6. Filter removal verification:
   - Deleted filter no longer appears in saved filters dropdown
   - Filter count updates if displayed
   - Other saved filters remain unaffected
7. Edge case handling:
   - Deleting last filter works correctly
   - Saved filters dropdown handles empty state appropriately
   - No errors when filter list becomes empty
8. Multiple deletions:
   - Can delete multiple filters in sequence
   - Each deletion works independently
   - No conflicts between sequential deletions
9. Accessibility compliance:
   - Modal is properly announced by screen readers
   - All buttons are keyboard navigable
   - Delete confirmation is clearly communicated
   - Proper focus management when modal opens/closes
   - Escape key closes modal without deleting
10. Data persistence:
    - Deleted filters are permanently removed from user's saved filters
    - Deletion persists across browser sessions
    - No recovery mechanism for accidentally deleted filters