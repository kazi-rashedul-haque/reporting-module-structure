**Title:** Verify delete functionality with maximum length dashboard names.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Create a test dashboard with a maximum length name (120 characters): "This is a very long dashboard name that contains exactly one hundred and twenty characters to test the maximum length limit".
4. Locate the long-named dashboard in the dashboard table.
5. Click on the More Actions button (three dots) for the dashboard.
6. Click on the Delete option from the dropdown menu.
7. Verify the Delete Dashboard modal opens.
8. Check that the full dashboard name is displayed correctly in the confirmation message.
9. Verify the modal layout accommodates the long name without UI breaking.
10. Click the Delete button to confirm deletion.
11. Verify the dashboard is deleted successfully.
12. Check that no truncation or display issues occur.

**Expected Result:**
Dashboards with maximum length names should be deletable without issues, the confirmation modal should display the full dashboard name correctly, the modal layout should accommodate long names without breaking the UI, the exact long dashboard name should be shown in the confirmation message, the deletion process should complete successfully, and no truncation or overflow should occur in the modal display.