**Title:** Verify pagination does not appear with 10 or fewer reports

**Preconditions:**
  1. Exactly 10 or fewer reports exist in the system.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Report List page.
  3. Verify that all available reports are displayed in the table.
  4. Check the bottom area of the report table for pagination controls.

**Expected Result:**
* No pagination controls are displayed when there are 10 or fewer reports
* All reports are visible on a single page
* No page navigation elements are shown
* The report table displays cleanly without unnecessary pagination UI