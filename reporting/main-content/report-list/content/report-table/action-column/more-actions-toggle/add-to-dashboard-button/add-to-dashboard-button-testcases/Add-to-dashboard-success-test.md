**Title:** Verify that clicking Add to Dashboard successfully adds the report to the selected dashboard

**Preconditions:**
  1. At least one dashboard exists in the system.
  2. At least one report exists that can be added to dashboards in the system.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Search for the report name
4. Select the specific report from the reports table.
5. Open the Add to Dashboard modal by clicking "More Actions" then "Add to Dashboard".
6. Search for and display available dashboards.
7. Select a target dashboard by clicking its checkbox.
8. Verify the "Add to Dashboard" button is enabled.
9. Click the "Add to Dashboard" button.
10. Observe the modal behavior and any loading indicators.
11. Wait for the operation to complete.
12. Check for success notifications or messages.
13. Navigate to the selected dashboard.
14. Verify the report appears in the dashboard's report list.
15. Confirm the report functions correctly within the dashboard.

**Expected Result:**
• Modal closes automatically after successful addition
• User returns to the Reports page without manual navigation
• Success message or toast notification appears confirming the addition
• Loading indicator shows during the process if applicable
• The selected dashboard is updated with the new report
• Report appears in the dashboard's report list with correct title and data
• Report maintains its original functionality when viewed in the dashboard
• Dashboard layout adjusts properly to accommodate the new report
• No error messages appear during the process
• Operation completes within reasonable time limits