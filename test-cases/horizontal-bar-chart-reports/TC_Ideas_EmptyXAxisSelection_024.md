# Title: Ideas_EmptyXAxisSelection_024

# Pre-Condition: User has access to Reporting app with proper permissions

# Test Steps:
1. Open the browser and navigate to: https://reporting.t1.ideascale.dev
2. Accept cookies if prompted
3. Log in with the following credentials:
   - Email: superuser@ideascale.me
   - Password: brewski01
4. Click on the "Apps" button in the header
5. Click on the "Reporting NEW - Beta" app
6. Wait for the Reporting app to load
7. Click on "Reports" in the left sidebar
8. Wait for the Reports page to load
9. Click on "Create Report" button
10. Fill in the report details:
    - Report Name: EDGE_EmptyXAxisSelection_024
    - Description: Edge case test for attempting to show results without selecting X-axis value
11. Click on "Next" to create the report
12. Select "Horizontal Bar" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Leave "X Axis" dropdown unselected (empty selection)
16. Select "Quarterly" from the "Y Axis" dropdown
17. Attempt to click on "Show Results" button
18. Verify that validation prevents showing results without X-axis selection
19. Verify appropriate error message or validation indicator appears
20. Select "# of Ideas Submitted" from the "X Axis" dropdown to resolve the validation
21. Verify validation error is cleared
22. Click on "Show Results" button
23. Verify "Save changes" button appears beside "Show Results" button
24. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
25. Click on "Save changes" button
26. Verify success message appears and disappears after a few seconds

# Expected Results:
- Initial attempt to show results without X-axis selection is prevented by validation
- Appropriate validation error message displayed indicating X-axis selection is required
- "Show Results" button is disabled or validation prevents action when X-axis is not selected
- Error message clearly indicates that X-axis value must be selected
- After selecting X-axis value, validation error is cleared
- Report saved successfully with name: "EDGE_EmptyXAxisSelection_024"
- Report description: "Edge case test for attempting to show results without selecting X-axis value"
- Success message displayed
- Chart type: Horizontal bar chart displayed correctly with horizontal bars
- X-Axis label: Shows "# of Ideas Submitted" metric name in the top-right corner of the chart
- Y-Axis label: Shows quarterly data points (Q1 2024, Q2 2024, Q3 2024, Q4 2024)
- First column of table: "Dataset" containing the X-axis value "# of Ideas Submitted"
- Subsequent columns: Q1 2024, Q2 2024, Q3 2024, Q4 2024 (for Quarterly)
- Cell values: Match the corresponding horizontal bar chart data points when hovered
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "EDGE_EmptyXAxisSelection_024"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list