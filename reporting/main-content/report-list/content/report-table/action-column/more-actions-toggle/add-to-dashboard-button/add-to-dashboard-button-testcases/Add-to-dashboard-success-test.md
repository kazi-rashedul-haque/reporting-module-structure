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
10. Check for success notifications or messages.
11. Navigate to the selected dashboard.
12. Verify the report appears in the dashboard's report list.

**Expected Result:**
* Modal closes after successful addition.
* Success message/notification appears.
* User is returned to Reports page.
* Report is added to the selected dashboard.