**Title:** Verify Show Results button becomes enabled when report configuration is modified

**Pre-conditions:**
* User is logged into the workspace as an authenticated user
* At least one report exists in the report list
* Report details page is accessible
* Show Results button is initially disabled

**Test Steps:**
1. Login to the workspace as an authenticated user.
1. Navigate to the Reporting page.
2. Select any existing report from the Reports table to open the report details page.
3. Verify the "Show Results" button is initially disabled.
4. Make a change to any report configuration setting (e.g., change Data Category, Time Frame, X-axis grouping, or Y-axis dataset).
5. Observe the "Show Results" button state immediately after making the configuration change.
8. Verify the "Save changes" button, "Actions" button, and "Unsaved Changes" drop-down are enabled.

**Expected Result:**
* The "Show Results" button should become enabled immediately after any configuration change is made.
* The button should change from greyed out to primary color styling (visually stands out).
* * The "Save changes" button, "Actions" button, and "Unsaved Changes drop-down" should all be enabled.