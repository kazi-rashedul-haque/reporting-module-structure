**Title:** Verify delete functionality with dashboards containing special characters.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Create test dashboards with names containing special characters: "Test@#$%Dashboard", "Dashboard with spaces", "Dashboard'with'quotes", "Dashboard<>&HTML".
4. Locate each test dashboard in the dashboard table.
5. For each dashboard, click on the More Actions button (three dots).
6. Click on the Delete option from the dropdown menu.
7. Verify the Delete Dashboard modal opens with the exact dashboard name displayed correctly.
8. Confirm the special characters are properly rendered in the confirmation message.
9. Click the Delete button to confirm deletion.
10. Verify each dashboard is successfully deleted.
11. Check that no encoding issues or display problems occur.

**Expected Result:**
Dashboards with special characters should be deletable without issues, the confirmation modal should display all special characters correctly without encoding problems, the exact dashboard name should be shown in the confirmation message regardless of special characters, the deletion process should complete successfully for all special character combinations, and no HTML injection or display issues should occur.