**Title:** Verify delete button opens confirmation modal with correct report name.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Locate a user-created report in the report table and note its name.
4. Click on the More Actions button (three dots) for the report.
5. Click on the Delete option from the dropdown menu.
6. Verify the Delete Report modal opens.
7. Check the modal title displays "Delete Report".
8. Verify the body text contains the exact report name in the confirmation message.
9. Confirm the message follows the format: "Are you sure you want to delete '<report_name>'?"
10. Verify the modal has Cancel and Delete buttons.

**Expected Result:**
The Delete Report modal should open immediately when the Delete option is clicked, the modal title should be "Delete Report", the confirmation message should include the exact report name in the specified format, and the modal should contain Cancel and Delete action buttons.