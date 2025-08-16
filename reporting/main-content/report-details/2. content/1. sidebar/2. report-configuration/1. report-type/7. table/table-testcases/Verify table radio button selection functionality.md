**Title:** Verify table radio button selection functionality

**Pre-conditions:**
* At least one report exists in the report list
* The sidebar is currently expanded

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Verify the "Report Type" section is visible in the Customization sidebar.
5. Locate the Table radio button with aria-label "Table" in the Report Type group.
6. Click on the Table radio button or its associated label.
7. Verify the Table radio button shows [checked] and [active] attributes.
8. Verify other report type radio buttons (Line, Bar, Horizontal Bar, Dual Axis, Metric Card, Donut) are unchecked.
9. Verify Table-specific configuration options appear: Data Category combobox, Time Frame button, Data Grouping combobox showing "Choose Data", Dataset section with "Add Dataset" button.

**Expected Result:**
* Table radio button should display [checked] and [active] attributes in DOM
* Other report type radio buttons (Line, Bar, Horizontal Bar, Dual Axis, Metric Card, Donut) should be unchecked
* Table-specific customization options should be visible and functional:
  - Data Category combobox with current selection displayed
  - Time Frame button (e.g., "Last 30 Days")
  - Data Grouping combobox showing "Choose Data" as placeholder
  - Dataset section with "Choose" placeholder and "Add Dataset" button
  - Add Filter button in Filters section
* Show Results button should become enabled when configuration is complete
* Main content area should display data table with appropriate columns and rows