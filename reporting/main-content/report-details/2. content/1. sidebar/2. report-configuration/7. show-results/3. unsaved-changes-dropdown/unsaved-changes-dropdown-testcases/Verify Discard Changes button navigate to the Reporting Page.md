**Title:** Verify Discard Changes button navigate to the Reporting Page

**Pre-conditions:**
* At least one report exists in the report list
* Unsaved Changes Warning Modal is displayed with unsaved changes

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Note the original report configuration state.
5. Modify the report configuration (e.g., changing report type, axis, or dataset).
6. Do not save the changes.
7. Attempt to navigate away from the report page to trigger the warning modal.
8. Click the "Discard Changes" button in the modal.

**Expected Result:**
* Clicking "Discard Changes" should confirm back to the Reporting Page.
