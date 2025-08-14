**Title:** Verify Cancel button works with empty fields.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Ensure both Report Name and Description fields are empty.
5. Click the Cancel button.
6. Verify the modal closes immediately.
7. Verify the user returns to the Reports page.

**Expected Result:**
The modal should close immediately when the Cancel button is clicked even with empty fields, the user should return to the Reports page without any errors or unexpected behavior, and the Cancel button should function normally regardless of whether fields contain data or are empty.