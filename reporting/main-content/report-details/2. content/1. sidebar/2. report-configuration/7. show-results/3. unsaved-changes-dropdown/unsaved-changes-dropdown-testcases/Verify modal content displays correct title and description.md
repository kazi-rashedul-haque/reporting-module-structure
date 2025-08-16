**Title:** Verify modal content displays correct title and description

**Pre-conditions:**
* At least one report exists in the report list
* Unsaved Changes Warning Modal is displayed

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Modify the report configuration (e.g., changing report type, axis, or dataset).
5. Do not save the changes.
6. Attempt to navigate away from the report page to trigger the warning modal.
7. Verify the modal title displays exactly "You have unsaved changes".
8. Verify the modal description states "Click `Continue Editing` to keep editing or `Discard Changes` to abandon changes."
9. Verify both actionable buttons are present: "Continue Editing" and "Discard Changes".

**Expected Result:**
* Modal title should display exactly "You have unsaved changes".
* Modal description should state exactly "Click `Continue Editing` to keep editing or `Discard Changes` to abandon changes."
* Both "Continue Editing" and "Discard Changes" buttons should be visible and actionable.