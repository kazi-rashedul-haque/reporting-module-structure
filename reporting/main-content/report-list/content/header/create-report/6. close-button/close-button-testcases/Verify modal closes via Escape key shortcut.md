**Title:** Verify modal closes via Escape key shortcut.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter "Test Report" in the Report Name field.
5. Enter "Test description" in the Description field.
6. Press the Escape key on the keyboard.
7. Verify the modal closes immediately.
8. Click the Create Report button again to reopen the modal.
9. Verify both fields are empty and data was discarded.

**Expected Result:**
The modal should close when the Escape key is pressed, all entered data should be completely discarded, the user should return to the Reports page, the Escape key should work identically to clicking the Close button, and when the modal is reopened, all fields should be empty with no persisted data.