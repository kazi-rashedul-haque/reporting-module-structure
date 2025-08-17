**Title:** Verify clone button prevents double submission with rapid clicks

**Preconditions:**
  1. User is authenticated and has access to the reporting module.
  2. At least one report exists and is accessible in the report details page.
  3. User has permission to clone reports.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page and open any report.
3. Click on the "Actions" dropdown button to open the menu.
4. Rapidly click on the "Clone" button multiple times in quick succession. .
5. Verify that only one clone operation is processed.
6. Check that no duplicate reports are created

**Expected Result:**
• Only one clone operation is processed regardless of multiple clicks
• Clone button becomes disabled or non-responsive after first click until operation completes
• No duplicate reports are created in the system