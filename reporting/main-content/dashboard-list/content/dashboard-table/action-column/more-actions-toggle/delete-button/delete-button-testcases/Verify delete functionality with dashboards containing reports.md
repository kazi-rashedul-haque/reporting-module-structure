**Title:** Verify delete functionality with dashboards containing reports.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Create a test dashboard and note its name.
4. Add multiple reports to the test dashboard.
5. Verify the dashboard contains the added reports.
6. Click on the More Actions button (three dots) for the dashboard.
7. Click on the Delete option from the dropdown menu.
8. Verify the Delete Dashboard modal opens.
9. Check if any warning message appears about the dashboard containing reports.
10. Click the Delete button to confirm deletion.
11. Verify the dashboard is deleted successfully.
12. Navigate to the Reports page to verify that the reports that were in the deleted dashboard are still available and not affected by the dashboard deletion.

**Expected Result:**
Dashboards containing reports should be deletable, the system should either provide a warning about the dashboard containing reports or handle the deletion gracefully, the deletion should complete successfully, and the reports that were contained in the deleted dashboard should remain available and unaffected in the Reports section.