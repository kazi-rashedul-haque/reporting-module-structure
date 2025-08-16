**Title:** Verify Cancel button functionality in Rename Report modal

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page and open any user-created report details.
3. Click on the "Actions" dropdown in the report details header.
4. Select the "Rename Report" option from the dropdown.
1. Open the Rename Report modal for a user-created report.
2. Note the original report name and description values.
3. Make changes to the report name field.
4. Make changes to the description field.
5. Click the Cancel button.
6. Verify the modal closes immediately.
7. Reopen the Rename Report modal.
8. Verify original values are preserved in both fields.
9. Test Cancel button without making any changes to confirm it works.
10. Verify Cancel button is always enabled regardless of field content.
11. Check that focus returns appropriately after modal closure.

**Expected Result:**
* Cancel button is always enabled and never disabled
* Clicking Cancel closes the modal immediately without any confirmation dialog
* No changes are saved to the report when Cancel is clicked
* Original report name and description remain unchanged after cancellation
* Modal can be reopened with original values intact in both fields
* Focus returns to the appropriate element (Rename button) when modal closes
* Cancel functionality works consistently whether changes were made or not