**Title:** Verify Discard Changes Button reverts report to last saved state

**Pre-conditions:**
* At least one user report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Note the original report configuration state (report type, axis, dataset, etc.).
5. Modify the report configuration (e.g., changing report type, axis, or dataset).
6. Do not save the changes.
7. Click on the "Unsaved Changes"dropdown in the top-right corner.
8. Click the "Discard Changes" button in the dropdown.

**Expected Result:**
* The current unsaved changes should be discarded immediately.
* The report should revert to the last saved state with all original configuration settings restored.
* The "Unsaved Changes" button should disappear from the interface.