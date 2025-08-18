**Title:** Verify Last Updated column sorting functionality in ascending order

**Preconditions:**
1. Multiple dashboards exist in the dashboards table with varying last updated dates.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Locate the "Last Updated" column header.
4. Hover over the column header and verify cursor changes to pointer.
5. Click on the column header once.
6. Verify that the click action triggers sorting behavior (check for sort indicator).
7. Verify the actual sorting of data (ascending/descending order).

**Expected Results:**
* The Last Updated column header should display pointer cursor on hover
* First click should sort data in ascending order with up arrow indicator (↑)
* Second click should sort data in descending order with down arrow indicator (↓)