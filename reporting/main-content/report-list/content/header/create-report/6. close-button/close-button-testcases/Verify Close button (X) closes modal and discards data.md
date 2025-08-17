**Title:** Verify Close button (X) closes modal and discards data.

**Test Steps:**
1. Login to the Workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter "Test Report Name" in the Report Name field.
5. Enter "Test description text" in the Description field.
6. Click the Close button (X) in the modal header.
7. Verify the modal closes immediately.
8. Click the Create Report button again to reopen the modal.
9. Verify both Report Name and Description fields are empty.

**Expected Result:**
The modal should close immediately when the Close button is clicked, all entered data should be completely discarded, the user should return to the Reports page, and when the modal is reopened, all fields should be empty with no data persisted from the previous session.