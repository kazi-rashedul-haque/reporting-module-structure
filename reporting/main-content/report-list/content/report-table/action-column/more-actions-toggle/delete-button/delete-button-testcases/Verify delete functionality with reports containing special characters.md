**Title:** Verify delete functionality with reports containing special characters.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Create test reports with names containing special characters: "Test@#$%Report", "Report with spaces", "Report'with'quotes", "Report<>&HTML".
4. Locate each test report in the report table.
5. For each report, click on the More Actions button (three dots).
6. Click on the Delete option from the dropdown menu.
7. Verify the Delete Report modal opens with the exact report name displayed correctly.
8. Confirm the special characters are properly rendered in the confirmation message.
9. Click the Delete button to confirm deletion.
10. Verify each report is successfully deleted.
11. Check that no encoding issues or display problems occur.

**Expected Result:**
Reports with special characters should be deletable without issues, the confirmation modal should display all special characters correctly without encoding problems, the exact report name should be shown in the confirmation message regardless of special characters, the deletion process should complete successfully for all special character combinations, and no HTML injection or display issues should occur.