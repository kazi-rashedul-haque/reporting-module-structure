**Title:** Verify Show Results button behavior with incomplete configuration

**Pre-conditions:**
* At least one report exists in the report list
* The sidebar is currently expanded
* Table radio button is selected

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Select Table from the Report Type options.
5. Leave Data Grouping as "Choose Data" or Dataset as "Choose" (incomplete configuration).
6. Locate the "Show Results" button in the customization sidebar.
7. Verify the Show Results button is disabled when configuration is incomplete.
8. Complete the required configuration: select Data Grouping and Dataset values.
9. Verify the Show Results button becomes enabled.
10. Click Show Results and verify the data table updates with new configuration.

**Expected Result:**
* Show Results button should be disabled when required fields are incomplete
* Button should display visual disabled state (grayed out, non-clickable)
* Completing required configuration (Data Category, Data Grouping, Dataset) should enable the button
* Enabled Show Results button should be clickable and trigger table data update
* Data table should refresh with new data based on configuration parameters
* No validation messages needed as button state prevents invalid submissions