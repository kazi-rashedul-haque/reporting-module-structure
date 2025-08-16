**Title:** Verify metric card radio button selection functionality

**Pre-conditions:**
* At least one report exists in the report list
* The sidebar is currently expanded

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Verify the Report Type section is visible in the sidebar.
5. Locate the Metric Card radio button option.
6. Click on the Metric Card radio button.
7. Verify the radio button becomes selected (checked state).
8. Verify other report type options become deselected.

**Expected Result:**
* Metric Card radio button should be selected and show checked state
* Other report type radio buttons should be deselected
* Metric Card specific customization options should appear including Data Category, Time Frame, Data Grouping, Dataset, and Add Filter
* Selection should be visually indicated with appropriate styling