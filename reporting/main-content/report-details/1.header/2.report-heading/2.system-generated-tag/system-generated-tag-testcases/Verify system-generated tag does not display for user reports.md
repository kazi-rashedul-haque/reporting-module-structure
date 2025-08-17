**Title:** Verify system-generated tag does not display for user reports

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Select a user-created report from the reports table (shows "You" in Created by column).
4. Open the report details page.
5. Examine the header section where the system-generated tag would appear.
6. Verify that no "System Generated" tag is displayed.

**Expected Result:**
* The "System Generated" tag should NOT be visible for user-created reports.
* The header layout should display cleanly without the tag.