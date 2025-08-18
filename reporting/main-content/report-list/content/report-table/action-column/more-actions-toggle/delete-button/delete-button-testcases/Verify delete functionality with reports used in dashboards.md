**Title:** Verify delete functionality with reports used in dashboards.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Create a test report and note its name.
4. Navigate to the Dashboard section and add the test report to a dashboard.
5. Return to the Reports page.
6. Locate the test report and verify it shows "X Dashboard(s)" in the Used in column.
7. Click on the More Actions button (three dots) for the report.
8. Click on the Delete option from the dropdown menu.
9. Verify the Delete Report modal opens.
10. Check if any warning message appears about the report being used in dashboards.
11. Click the Delete button to confirm deletion.
12. Verify the report is deleted successfully.
13. Navigate to the dashboard where the deleted report was previously added to verify the impact and confirm proper handling of the missing report.

**Expected Result:**
Reports used in dashboards should still be deletable, the system should either provide a warning about dashboard usage or handle the deletion gracefully, the deletion should complete successfully, and the dashboard should handle the removal of the deleted report appropriately (either by removing the report card or showing an error state).