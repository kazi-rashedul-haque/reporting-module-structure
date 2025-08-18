**Title:** Verify that the Add to Dashboard button states change correctly based on selection

**Preconditions:**
1. Add to Dashboard modal is open with dashboard options visible.
2. At least one dashboard option is available for selection.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Search for a specific report in the reports table.
4. Click on the "More Actions" toggle for the selected report.
5. Click on the "Add to Dashboard" button from the dropdown menu.
6. Verify the Add to Dashboard modal opens successfully.
7. Search for and display available dashboards.
8. Select a dashboard by clicking its checkbox.
9. Observe the "Add to Dashboard" button state change.
11. Deselect the dashboard checkbox by clicking it again.
12. Verify the button returns to disabled state.



**Expected Result:**
1. "Add to Dashboard" button is initially disabled with grayed-out appearance and non-clickable state
2. Button becomes enabled immediately when at least one dashboard is selected
3. Button text may update to reflect selection count (e.g., "Add to Dashboard" or "Add to 2 Dashboards")
4. Button becomes disabled again when all selections are removed
5. Button visual state changes clearly indicate enabled/disabled status 
6. Button hover effects work appropriately when enabled
7. Button remains consistently disabled when no valid selections exist