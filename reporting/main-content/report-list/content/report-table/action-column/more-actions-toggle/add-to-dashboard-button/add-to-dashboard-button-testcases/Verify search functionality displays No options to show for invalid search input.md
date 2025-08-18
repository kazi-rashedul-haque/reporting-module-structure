# Verify search functionality displays No options to show for invalid search input

**Title:** Verify search functionality displays No options to show for invalid search input

**Preconditions:**
  1. User is authenticated and logged into the system.
  2. Add to Dashboard modal is open and functional.
  3. Search functionality is enabled in the modal.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Search for a specific report in the reports table.
4. Click on the "More Actions" button for the report .
5. Select "Add to Dashboard" from the dropdown menu.
6. Then Add to Dashboard modal should open.
7. Click in the search textbox to focus on it.
8. Enter an invalid search term that doesn't match any dashboard names (e.g., "xyz123invalid", "nonexistentdashboard", "@@@@").
9. Press Enter or wait for auto-search to trigger.
10. Observe the search results area.
11. Check the state of the "Add to Dashboard" button.
12. Verify the empty state message and icon are displayed.

**Expected Result:**
1. Search textbox accepts and displays the invalid input text
2. Search results area shows "No options to show" message clearly
3. Empty chart icon is displayed in the results area
4. "Add to Dashboard" button remains disabled throughout the process
5. No dashboard options appear in the results list