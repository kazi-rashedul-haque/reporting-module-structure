**Title:** Verify Save Changes Button saves configuration and shows success alert

**Pre-conditions:**
* At least one user report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Note the original report configuration state.
5. Modify the report configuration (e.g., changing report type, axis, or dataset).
6. Do not save the changes initially.
7. Click on the "Unsaved Changes" button in the top-right corner.
8. Click the "Save Changes" button in the dropdown.

**Expected Result:**
* The current report configuration should be saved successfully.
* A success alert/notification should be displayed confirming the update.
* The "Unsaved Changes" button should disappear from the interface.
* The modified configuration should persist when navigating away and returning to the report.
* The user should remain on the same report details page.