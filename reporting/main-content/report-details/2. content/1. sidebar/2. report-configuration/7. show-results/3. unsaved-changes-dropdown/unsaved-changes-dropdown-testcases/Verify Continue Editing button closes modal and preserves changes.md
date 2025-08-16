**Title:** Verify Continue Editing button closes modal and preserves changes

**Pre-conditions:**
* At least one report exists in the report list
* Unsaved Changes Warning Modal is displayed with unsaved changes

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Modify the report configuration (e.g., changing report type, axis, or dataset).
5. Do not save the changes.
6. Attempt to navigate away from the report page to trigger the warning modal.
7. Click the "Continue Editing" button in the modal.
8. Verify the modal closes.
9. Verify the user can continue editing the report.
10. Verify no changes are discarded and all modifications remain visible.

**Expected Result:**
* Clicking "Continue Editing" should close the modal.
* No changes should be discarded.
* All previous modifications should remain visible and editable.