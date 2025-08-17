**Title:** Verify delete modal cancel button functionality.

**Preconditions:**
1. User created dashboard exists in the dashboard table.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Dashboard List page.
3. Locate a user-created dashboard in the dashboard table.
4. Click on the More Actions button (three dots) for the dashboard.
5. Click on the Delete option from the dropdown menu.
6. Verify the Delete Dashboard modal opens.
7. Click the Cancel button in the modal.
8. Verify the modal closes immediately.
9. Confirm the user returns to the Dashboard List page.


**Expected Result:**
The Cancel button should close the Delete Dashboard modal immediately without performing any deletion action, the user should return to the Dashboard List page.