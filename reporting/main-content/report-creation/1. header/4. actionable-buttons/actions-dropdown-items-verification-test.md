**Title:** Verify Actions dropdown displays all menu items with correct enabled/disabled states

**Pre-conditions:**
* User is logged in as an authenticated user with reporting access

**Test Steps:**
1. Navigate to the "Reporting" application
2. Open an existing report for editing
3. Click on the "Actions" button to open the dropdown menu
4. Verify all menu items are displayed in the dropdown
5. Verify which items are enabled and which are disabled
6. Click outside the dropdown to close it

**Expected Results:**
* Dropdown displays the following menu items: "Add to Dashboard", "Export to CSV", "Export to Excel", "Rename", "Schedule Email Report", "Add to Favorites", "Clone", "Delete"
* Enabled items: "Add to Dashboard", "Rename", "Add to Favorites" OR "Remove from Favorites" (depending on current favorite status), "Clone", "Delete"
* Disabled items (with "Upcoming" labels): "Export to CSV", "Export to Excel", "Schedule Email Report"
* The "Actions" dropdown menu will be closed when clicking outside of it