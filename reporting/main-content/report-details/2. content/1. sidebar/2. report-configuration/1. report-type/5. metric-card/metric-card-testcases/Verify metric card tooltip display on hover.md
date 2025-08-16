**Title:** Verify metric card tooltip display on hover

**Pre-conditions:**
* At least one report exists in the report list
* The sidebar is currently expanded

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Locate the Metric Card option in the Report Type section.
5. Hover over the Metric Card option without clicking.
6. Verify tooltip appears displaying "Metric Card".
7. Move cursor away from the Metric Card option.
8. Verify tooltip disappears.

**Expected Result:**
* Tooltip should appear immediately when hovering over Metric Card option
* Tooltip should display "Metric Card" text clearly
* Tooltip should disappear when cursor moves away
* Tooltip behavior should be consistent across multiple hover interactions