**Test Case:** Verify special characters handling correctly

**Precondition:**
1. A report with special characters in its name exists in the Reports table.

**Test Steps:**
1. Login to the workspace as a valid user.
2. Go to the Reports page.
3. Select a report that has special characters in its name (e.g., Report_123!@#).
4. Open the report details page.
5. Check the report name shown in the header.

**Expected Result:**
* The report name should appear exactly as created (with all special characters, numbers, and symbols).
* Header formatting should remain consistent without distortion.