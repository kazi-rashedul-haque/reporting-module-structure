**Title:** Verify Add Filter functionality for dual-axis chart

**Pre-conditions:**
* User is logged in to the workspace
* At least one report exists with dual-axis chart type configured
* All basic chart configurations are set (Data Category, Time Frame, X Axis, Y Axes)

**Test Steps:**
1. Navigate to the Reporting page.
2. Select an existing report to open the report details page.
3. In the sidebar, ensure "Dual-axis" chart type is selected.
4. Locate the "Add Filter" option in the configuration panel.
5. Click on "Add Filter" to open filter options.
6. Verify the filter interface displays available filter criteria options.
7. Select a filter type (e.g., status, category, member properties).
8. Configure filter values or conditions for the selected filter type.
9. Apply the filter and verify the chart updates to reflect filtered data.
10. Verify both bar and line chart components respect the applied filter.
11. Check that the chart legend and axes adjust appropriately for filtered data.
12. Add multiple filters and verify they work in combination.
13. Test removing individual filters and verify chart updates accordingly.
14. Verify filter summary or indicators are displayed in the configuration panel.

**Expected Result:**
* "Add Filter" option is accessible and functional
* Filter interface displays all available filter criteria
* Filter configuration options work correctly for different filter types
* Chart updates dynamically when filters are applied
* Both bar and line chart components reflect filtered data accurately
* Multiple filters can be applied and work in combination
* Filter removal functionality works correctly
* Chart axes and scaling adjust appropriately for filtered data ranges
* Filter indicators or summaries are clearly displayed
* Filtered chart maintains proper dual-axis functionality and readability