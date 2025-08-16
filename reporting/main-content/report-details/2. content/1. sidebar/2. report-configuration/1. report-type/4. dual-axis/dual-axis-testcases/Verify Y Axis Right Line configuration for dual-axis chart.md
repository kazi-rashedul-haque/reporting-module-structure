**Title:** Verify Y Axis Right Line configuration for dual-axis chart

**Pre-conditions:**
* User is logged in to the workspace
* At least one report exists with dual-axis chart type configured
* Data Category, Time Frame, X Axis, and Y Axis Left (Bar) are already configured

**Test Steps:**
1. Navigate to the Reporting page.
2. Select an existing report to open the report details page.
3. In the sidebar, ensure "Dual-axis" chart type is selected.
4. Locate the "Y Axis Right (Line)" configuration option.
5. Click on the "Y Axis Right (Line)" dropdown to view available options.
6. Verify the dropdown shows Ideas or Members Data Grouping values.
7. Select a specific data grouping value from the dropdown.
8. Verify the right Y-axis displays appropriate scale and labels for the selected data.
9. Verify the line chart component updates to reflect the selected Y-axis data.
10. Check that the right Y-axis scale adjusts automatically based on data range.
11. Verify the line chart uses distinct colors and line styles.
12. Test the "Add Dataset" option appears for the Y Axis Right (Line).
13. Click "Add Dataset" and verify it shows all available values except the currently selected one.
14. Verify both left and right Y-axes display simultaneously with proper scaling.

**Expected Result:**
* Y Axis Right (Line) dropdown displays all available Ideas or Members Data Grouping values
* Right Y-axis updates with appropriate scale and labels when selection changes
* Line chart displays correctly with proper scaling and positioning
* Line chart uses distinct, accessible colors and line styles
* Right Y-axis scale automatically adjusts independently from left Y-axis
* "Add Dataset" option is available and functional
* Add Dataset dropdown excludes currently selected values
* Both Y-axes display simultaneously without interference
* Chart maintains proper dual-axis scaling and readability