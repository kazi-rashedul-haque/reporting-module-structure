**Title:** Verify Last Updated column sorting functionality in descending order

**Preconditions:**
1. Multiple reports exist in the reports table with varying last updated dates.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to reportingPage.
3. Click on the "Last updated on" column header once to sort ascending.
4. Click on the "Last updated on" column header again to sort descending.
5. Examine the order of reports in the table.
6. Verify the reports are sorted by last updated date in reverse chronological order (newest first).

**Expected Result:**
* The "Last updated on" column should sort reports in descending chronological order when clicked twice.
* Column header should maintain active state when sorting is applied.
* Reports with newer last updated dates should appear first.
* The sorting should reverse the order from the ascending sort.