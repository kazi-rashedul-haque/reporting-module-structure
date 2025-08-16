# Title: Ideas_CustomRange_IdeaStageChange_014

# Pre-Condition: User has access to Reporting app with proper permissions

# Test Steps:
1. Open the browser and navigate to: https://reporting.t1.ideascale.dev
2. Accept cookies if prompted
3. Log in with the following credentials:
   - Email: superuser@ideascale.me
   - Password: brewski01
4. Click on the "Apps" button in the header
5. Click on the "Reporting" app
6. Wait for the Reporting app to load
7. Click on "Reports" in the left sidebar
8. Wait for the Reports page to load
9. Click on "Create Report" button
10. Fill in the report details:
    - Report Name: REG_Ideas_CustomRange_IdeaStageChange_014
    - Description: Regression test for line chart with Ideas data category, Custom Range validation, and Idea Stage Change Y-axis
11. Click on "Next" to create the report
12. Select "Line" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Custom Range" from the "Time Frame" dropdown
15. Verify date picker appears with "Start Date" and "End Date"
16. Set Start Date to 30 days ago from current date
17. Set End Date to current date
18. Select "Quarterly" from the "X Axis" dropdown
19. Select "Idea Stage Change" from the "Y Axis" dropdown
20. Verify "Save changes" button is not visible yet
21. Click on "Show Results" button
22. Verify "Save changes" button appears beside "Show Results" button
23. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
24. Click on "Save changes" button
25. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "REG_Ideas_CustomRange_IdeaStageChange_014"
- Report description: "Regression test for line chart with Ideas data category, Custom Range validation, and Idea Stage Change Y-axis"
- Success message displayed
- Chart type: Line chart displayed correctly
- Custom date range functionality works correctly
- Date picker allows valid date selection
- X-Axis label: Shows quarterly data points for the custom range
- Y-Axis label: Shows "Idea Stage Change" metric name in the top-right corner of the chart
- First column of table: "Dataset" containing the Y-axis value "Idea Stage Change"
- Subsequent columns: Based on the custom date range selected
- Cell values: Match the corresponding line chart data points when hovered
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "REG_Ideas_CustomRange_IdeaStageChange_014"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list