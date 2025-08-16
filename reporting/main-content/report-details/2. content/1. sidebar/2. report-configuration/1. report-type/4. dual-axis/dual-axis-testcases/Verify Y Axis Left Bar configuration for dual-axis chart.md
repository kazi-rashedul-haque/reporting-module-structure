**Title:** Verify Y Axis Left Bar configuration for dual-axis chart

**Pre-conditions:**
* User is logged in to the workspace
* At least one report exists with dual-axis chart type configured
* Data Category, Time Frame, and X Axis are already configured

**Test Steps:**
1. Navigate to the Reporting page.
2. Select an existing report to open the report details page.
3. In the sidebar, ensure "Dual-axis" chart type is selected.
4. Locate the "Y Axis Left (Bar)" configuration option.
5. Click on the "Y Axis Left (Bar)" dropdown to view available options.
6. Verify the dropdown shows Ideas or Members Data Grouping values.
7. Select a specific data grouping value from the dropdown.
8. Verify the left Y-axis displays appropriate scale and labels for the selected data.
9. Verify the bar chart component updates to reflect the selected Y-axis data.
10. Check that the left Y-axis scale adjusts automatically based on data range.
11. Verify the bar chart colors are distinct and visible.
12. Test the "Add Dataset" option appears for the Y Axis Left (Bar).
13. Click "Add Dataset" and verify it shows all available values except the currently selected one.

**Expected Result:**
* Y Axis Left (Bar) dropdown displays all available Ideas or Members Data Grouping values
* Left Y-axis updates with appropriate scale and labels when selection changes
* Bar chart displays correctly with proper scaling and positioning
* Bar chart uses distinct, accessible colors
* Left Y-axis scale automatically adjusts to accommodate data range
* "Add Dataset" option is available and functional
* Add Dataset dropdown excludes currently selected values
* Bar chart legend updates to reflect the selected data grouping