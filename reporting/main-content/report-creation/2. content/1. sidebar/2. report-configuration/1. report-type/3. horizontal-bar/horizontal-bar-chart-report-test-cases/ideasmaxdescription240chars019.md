# Title: Ideas_MaxDescription_240Chars_019

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
    - Report Name: EDGE_MaxDescription_240Chars_019
    - Description: Edge case test for maximum description length exactly 240 characters with horizontal bar chart Ideas data category # of Ideas Submitted X-axis and Quarterly Y-axis testing character limit validation functionality working
11. Verify character counter shows 240/240 for description
12. Click on "Next" to create the report
13. Select "Horizontal Bar" as the "Report Type"
14. Select "Ideas" from the "Data Category" dropdown
15. Select "Last 365 Days" from the "Time Frame" dropdown
16. Select "# of Ideas Submitted" from the "X Axis" dropdown
17. Select "Quarterly" from the "Y Axis" dropdown
18. Verify "Save changes" button is not visible yet
19. Click on "Show Results" button
20. Verify "Save changes" button appears beside "Show Results" button
21. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
22. Click on "Save changes" button
23. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "EDGE_MaxDescription_240Chars_019"
- Report description: "Edge case test for maximum description length exactly 240 characters with horizontal bar chart Ideas data category # of Ideas Submitted X-axis and Quarterly Y-axis testing character limit validation functionality working"
- Success message displayed
- Character counter correctly shows 240/240 for description
- System accepts exactly 240 characters for report description
- Chart type: Horizontal bar chart displayed correctly with horizontal bars
- X-Axis label: Shows "# of Ideas Submitted" metric name in the top-right corner of the chart
- Y-Axis label: Shows quarterly data points (Q1 2024, Q2 2024, Q3 2024, Q4 2024)
- First column of table: "Dataset" containing the X-axis value "# of Ideas Submitted"
- Subsequent columns: Q1 2024, Q2 2024, Q3 2024, Q4 2024 (for Quarterly)
- Cell values: Match the corresponding horizontal bar chart data points when hovered
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back with full description preserved

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "EDGE_MaxDescription_240Chars_019"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list