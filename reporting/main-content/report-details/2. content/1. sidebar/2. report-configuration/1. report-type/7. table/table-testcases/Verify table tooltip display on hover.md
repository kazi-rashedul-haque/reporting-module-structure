**Title:** Verify table tooltip display on hover

**Pre-conditions:**
* At least one report exists in the report list
* Table is displayed with data
* Table has multiple rows and columns

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Select Table and configure it to display data with Show Results.
5. Locate the data table in the main content area with rowgroup headers and data rows.
6. Hover the mouse cursor over different table cells containing data values.
7. Verify tooltip appears when hovering over table cells (if content is truncated or has additional info).
8. Verify tooltip displays relevant information for the hovered cell (date, value, dataset name).
9. Move cursor to different cells in header row and data rows.
10. Move cursor away from table and verify tooltip disappears.
11. Test tooltip positioning and readability across different cell types.

**Expected Result:**
* Tooltip should appear when hovering over table cells that have additional information or truncated content
* Tooltip should display relevant information: cell value, date/time details, dataset information
* Tooltip should update appropriately when moving between different cells
* Tooltip should disappear when cursor moves away from table area
* Tooltip content should be clearly formatted and readable
* Header cells and data cells may have different tooltip behaviors
* Table cells with generic elements containing values should show appropriate hover states