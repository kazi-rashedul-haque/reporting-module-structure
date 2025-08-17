**Title:** Verify delete button opens confirmation modal with correct dashboard name.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Dashboard List page.
3. Locate a user-created dashboard in the dashboard table and note its name.
4. Click on the More Actions button (three dots) for the dashboard.
5. Click on the Delete option from the dropdown menu.
6. Verify the Delete Dashboard modal opens.
7. Check the modal title displays "Delete Dashboard".
8. Verify the body text contains the exact dashboard name in the confirmation message.
9. Confirm the message follows the format: "Are you sure you want to delete '<dashboard_name>'?"
10. Verify the modal has Cancel and Delete buttons.

**Expected Result:**
The Delete Dashboard modal should open immediately when the Delete option is clicked, the modal title should be "Delete Dashboard", the confirmation message should include the exact dashboard name in the specified format, and the modal should contain Cancel and Delete action buttons.