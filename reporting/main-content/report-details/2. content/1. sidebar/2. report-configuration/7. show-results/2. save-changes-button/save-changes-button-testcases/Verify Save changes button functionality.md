**Title:** Verify Save changes button functionality

**Pre-conditions:**
* At least one user report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing user report from the Reports table to open the report details page.
4. Make changes to the report configuration
5.    (e.g., change Data Category, Time Frame, X-axis grouping, or Y-axis dataset).
6. Click the "Show Results" button to trigger report generation.
7. Wait for the report to generate and display results.
8. Click the "Save changes" button.
9. Wait for the save operation to complete.
10. Verify the success alert is displayed.

**Expected Result:**
* The "Save changes" button should be enabled after making configuration changes.
* The Success alert should appear after clicking "Save changes".