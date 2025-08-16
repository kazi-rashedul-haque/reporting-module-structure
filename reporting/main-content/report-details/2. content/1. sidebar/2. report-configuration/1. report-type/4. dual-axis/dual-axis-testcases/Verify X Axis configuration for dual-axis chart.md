**Title:** Verify X Axis configuration for dual-axis chart

**Pre-conditions:**
* User is logged in to the workspace
* At least one report exists with dual-axis chart type configured
* Data Category and Time Frame are already selected

**Test Steps:**
1. Navigate to the Reporting page.
2. Select an existing report to open the report details page.
3. In the sidebar, ensure "Dual-axis" chart type is selected.
4. Locate the "X Axis" configuration option.
5. Click on the "X Axis" dropdown to view available options.
6. Verify the dropdown shows "Time Properties", "Idea Properties", and "Member Properties" options.
7. Select "Time Properties" and verify the chart X-axis updates to show time-based labels.
8. Select "Idea Properties" and verify the chart X-axis updates to show idea-related property labels.
9. Select "Member Properties" and verify the chart X-axis updates to show member-related property labels.
10. For each X-axis selection, verify that both bar and line chart components align properly.
11. Check that the X-axis labels are readable and properly formatted.
12. Verify tooltip functionality when hovering over X-axis labels.

**Expected Result:**
* X Axis dropdown displays "Time Properties", "Idea Properties", and "Member Properties" options
* Chart X-axis updates dynamically when different axis types are selected
* X-axis labels display correctly formatted values for each property type
* Both bar and line chart components align properly with the X-axis
* X-axis labels are readable and don't overlap
* Tooltips provide additional information when hovering over X-axis elements
* Chart maintains proper scaling and spacing for all X-axis configurations