**Title:** Verify search functionality displays dashboard options for valid search input

**Preconditions:**
  1. At least created one dashboard exists 

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Search for a specific report in the reports table.
  4. Click on the "More Actions" toggle for the selected report.
  5. Click on the "Add to Dashboard" button from the dropdown menu.
  6. Verify the Add to Dashboard modal opens.
  7. Click in the search textbox to focus on it.
  8. Enter a valid dashboard name or partial name.
  9. Press Enter or wait for auto-search to trigger.
  10. Observe the search results area for matching dashboards.
  11. Verify that each dashboard option has a checkbox for selection.
  12. Check that dashboard names are displayed correctly.
  13. Ensure the "Add to Dashboard" button state before any selection.

**Expected Result:**
  Search textbox accepts and displays the valid input text,
  search results display a list of matching dashboards based on the search criteria
  each dashboard option appears with a selectable checkbox, dashboard names are clearly visible and properly formatted, search is case-insensitive and supports partial matching, "Add to Dashboard" button remains disabled until at least one dashboard is selected, search results update dynamically as user types, no "No options to show" message appears when valid results exist.

