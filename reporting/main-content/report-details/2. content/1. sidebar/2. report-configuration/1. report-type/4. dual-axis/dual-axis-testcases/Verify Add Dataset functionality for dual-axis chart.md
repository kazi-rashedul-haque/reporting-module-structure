**Title:** Verify Add Dataset functionality for dual-axis chart

**Pre-conditions:**
* At least one report exists with dual-axis chart type configured
* Data Category, Time Frame, X Axis, Y Axis Left (Bar), and Y Axis Right (Line) are already configured

**Test Steps:**
1. Login to the workspace as an authenticated user.
1. Navigate to the Reporting page.
2. Select an existing report to open the report details page.
3. In the sidebar, ensure "Dual-axis" chart type is selected.
4. Locate the "Add Dataset" option under "Y Axis Left (Bar)" configuration.
5. Click "Add Dataset" for the Y Axis Left (Bar).
7. Select an additional dataset from the dropdown.
9. Locate the "Add Dataset" option under "Y Axis Right (Line)" configuration.
10. Click "Add Dataset" for the Y Axis Right (Line).
11. Verify the dropdown shows all available data grouping values except the currently selected one.
12. Select an additional dataset from the dropdown.
13. Verify a new line series is added to the chart with a distinct color and line style.
14. Verify the chart legend updates to show all datasets with proper labels.
15. Test removing datasets by locating and clicking remove/delete options for added datasets.

**Expected Result:**
* "Add Dataset" options are available for both Y Axis Left (Bar) and Y Axis Right (Line)
* Add Dataset dropdowns exclude currently selected values
* New bar datasets appear with distinct, accessible colors
* New line datasets appear with distinct colors and line styles
* Chart legend updates to display all active datasets with clear labels
* Multiple datasets can be added to both bar and line components
* Remove/delete functionality works correctly for added datasets
* Chart maintains readability with multiple datasets displayed
* All datasets scale appropriately on their respective Y-axes