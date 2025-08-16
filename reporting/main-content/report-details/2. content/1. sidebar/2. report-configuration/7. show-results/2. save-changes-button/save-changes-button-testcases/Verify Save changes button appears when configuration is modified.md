**Title:** Verify Save changes button appears when configuration is modified

**Pre-conditions:**
* At least one user report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing user report from the Reports table to open the report details page.
4. Verify that no "Save changes" button is initially visible.
5. Make a change to any report configuration setting (e.g., change Report Type from Line to Bar, modify Data Category, Time Frame, X-axis grouping, or Y-axis dataset).
6. Observe the report configuration sidebar area immediately after making the change.
8. Click the "Show Results" button to trigger report generation.
10. Verify the "Save changes" button appears in the report configuration sidebar area.

**Expected Result:**
* The "Save changes" button should appear immediately after any configuration change is made.
* The button should display with outline styling and "Save changes" label.
* The "Save Changes" button should become enabled after clicking the Show Results Button.
* The button should only appear for user reports.