**Title:** Verify pagination appears when reports exceed 10 items

**Preconditions:**
  1. More than 10 reports exist in the system.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Verify that exactly 10 reports are displayed in the table.
  4. Verify that pagination controls appear at the bottom of the report table.
  5. Check that page numbers and navigation arrows are visible.

**Expected Result:**
* Pagination controls are displayed when there are more than 10 reports
* Only 10 reports are shown per page
* Page navigation elements (previous/next arrows, page numbers) are visible and functional
* Total page count is calculated correctly based on total number of reports