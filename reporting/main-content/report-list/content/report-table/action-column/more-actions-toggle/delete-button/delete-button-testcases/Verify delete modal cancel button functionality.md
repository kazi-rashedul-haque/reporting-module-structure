**Title:** Verify delete modal cancel button functionality.

**Preconditions:**
1. User created report exists in the report table.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Locate a user-created report in the report table.
4. Click on the More Actions button (three dots) for the report.
5. Click on the Delete option from the dropdown menu.
6. Verify the Delete Report modal opens.
7. Click the Cancel button in the modal.
8. Verify the modal closes immediately.
9. Confirm the user returns to the Reports page.


**Expected Result:**
The Cancel button should close the Delete Report modal immediately without performing any deletion action, the user should return to the Reports page.