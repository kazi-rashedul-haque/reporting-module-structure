**Title:** Verify Time Frame selection for dual-axis chart

**Pre-conditions:**
* User is logged in to the workspace
* At least one report exists with dual-axis chart type configured
* Data Category is already selected

**Test Steps:**
1. Navigate to the Reporting page.
2. Select an existing report to open the report details page.
3. In the sidebar, ensure "Dual-axis" chart type is selected.
4. Locate the "Time Frame" configuration option.
5. Click on the "Time Frame" dropdown to view available options.
6. Select a specific time frame (e.g., "Last 30 days", "Last 6 months", "Custom range").
7. If "Custom range" is selected, verify date picker functionality for start and end dates.
8. Verify the chart updates to display data within the selected time frame.
9. Check that both bar and line chart components reflect the time frame changes.
10. Verify the X-axis time labels update according to the selected time frame.

**Expected Result:**
* Time Frame dropdown displays all available time period options
* Chart updates dynamically when a new time frame is selected
* Date picker works correctly for custom time range selection
* Both bar and line chart data filters correctly to the selected time period
* X-axis displays appropriate time labels for the selected time frame
* Chart legend remains consistent with the time frame selection