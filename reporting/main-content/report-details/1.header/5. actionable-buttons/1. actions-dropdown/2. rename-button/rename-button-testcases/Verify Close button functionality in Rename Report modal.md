**Title:** Verify Close button functionality in Rename Report modal


**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page and open any user-created report details.
3. Click on the Actions dropdown and select "Rename Report".
1. Open the Rename Report modal for a user-created report.
2. Note the original report name and description values.
3. Make changes to both report name and description fields.
4. Click the Close button (X button) in the modal header.
5. Verify the modal closes immediately without any confirmation.
6. Reopen the Rename Report modal.
7. Verify original values are preserved in both fields.
8. Test Close button without making any changes to confirm functionality.
9. Verify Close button is always enabled regardless of field states.
10. Test keyboard accessibility by pressing ESC key (if supported).
11. Check that focus returns appropriately after modal closure.

**Expected Result:**
* Close button is always enabled and never disabled
* Clicking Close closes the modal immediately without any confirmation dialog
* No changes are saved to the report when Close button is clicked
* Original report name and description remain unchanged after closing
* Modal can be reopened with original values intact in both fields
* ESC key closes modal if keyboard accessibility is implemented
* Focus returns to the appropriate trigger element after modal closure
* Close functionality works consistently whether changes were made or not