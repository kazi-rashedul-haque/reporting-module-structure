**Title:** Verify report name updates after renaming elsewhere

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Select an existing report and open the report details page.
4. Note the current report name displayed in the header.
5. Navigate back to the Reports page.
6. Rename the report using the Actions dropdown or rename functionality.
7. Return to the report details page (refresh or re-navigate).
8. Verify the report name in the header reflects the new name.
9. Confirm the update is immediate and persistent.

**Expected Result:**
* The report name should update immediately after renaming.
* The new name should be displayed correctly in the report header.
* The change should persist across page refreshes and sessions.
* No caching issues should prevent the name update from showing.