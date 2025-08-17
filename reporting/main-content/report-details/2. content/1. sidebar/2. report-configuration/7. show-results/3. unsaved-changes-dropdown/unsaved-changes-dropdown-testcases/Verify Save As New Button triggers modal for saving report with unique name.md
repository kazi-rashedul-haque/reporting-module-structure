**Title:** Verify Save As New Button triggers modal for saving report with unique name

**Pre-conditions:**
* At least one user report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Note the original report configuration state.
5. Modify the report configuration (e.g., changing report type, axis, or dataset).
6. Do not save the changes.
7. Click on the "Unsaved Changes" button in the top-right corner.
8. Click the "Save As New" button in the dropdown.

**Expected Result:**
* A modal should appear prompting the user to enter a unique name for the new report.
* The modal should allow the user to save the current configuration as a new report.
* Upon successful save, the user should remain on the new report's details page.
* The original report should remain unchanged.