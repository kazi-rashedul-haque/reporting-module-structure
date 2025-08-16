**Title:** Verify line chart tooltip display on hover

**Pre-conditions:**
* At least one report exists in the report list
* The sidebar is currently expanded

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Locate the Line chart option in the Report Type section.
5. Hover over the Line chart option without clicking.
6. Verify tooltip appears displaying "Line".
7. Move cursor away from the Line chart option.
8. Verify tooltip disappears.
9. Repeat hover action to test consistency.

**Expected Result:**
* Tooltip should appear immediately when hovering over Line chart option
* Tooltip should display "Line" text clearly
* Tooltip should disappear when cursor moves away
* Tooltip behavior should be consistent across multiple hover interactions
* Hover state should provide visual feedback