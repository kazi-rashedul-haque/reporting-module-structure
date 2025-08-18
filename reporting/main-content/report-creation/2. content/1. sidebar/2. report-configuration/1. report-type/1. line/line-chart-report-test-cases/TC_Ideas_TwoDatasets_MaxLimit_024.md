# Title: Ideas_TwoDatasets_MaxLimit_024

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
    - Report Name: EDGE_Ideas_TwoDatasets_MaxLimit_024
    - Description: Edge case test for maximum dataset limit validation - testing that only 1 additional dataset can be added
11. Click on "Next" to create the report
12. Select "Line" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "X Axis" dropdown
16. Select "# of Ideas Submitted" from the "Y Axis" dropdown
17. Click on "Add Dataset" button
18. Select "# of Idea Views" from the new dropdown
19. Verify that no additional "Add Dataset" button appears (maximum 1 additional dataset reached)
20. Verify total of 2 Y-axis values are now configured
21. Verify "Save changes" button is not visible yet
22. Click on "Show Results" button
23. Verify "Save changes" button appears beside "Show Results" button
24. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
25. Click on "Save changes" button
26. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "EDGE_Ideas_TwoDatasets_MaxLimit_024"
- Report description: "Edge case test for maximum dataset limit validation - testing that only 1 additional dataset can be added"
- Maximum dataset limit validation works correctly - only 1 additional dataset can be added
- No additional "Add Dataset" button appears after adding the first additional dataset
- Total of 2 Y-axis values (original + 1 additional) are configured
- Success message displayed
- Chart type: Line chart displayed correctly with two lines
- X-Axis label: Shows quarterly data points (Q1 2024, Q2 2024, Q3 2024, Q4 2024)
- Y-Axis label: Shows both "# of Ideas Submitted" and "# of Idea Views" metric names in the top-right corner of the chart
- First row of table: "Dataset" containing "# of Ideas Submitted"
- Second row of table: "Dataset" containing "# of Idea Views"
- Subsequent columns: Q1 2024, Q2 2024, Q3 2024, Q4 2024 (for Quarterly)
- Cell values: Match the corresponding line chart data points when hovered
- Each dataset appears as a separate line in the chart with different colors
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "EDGE_Ideas_TwoDatasets_MaxLimit_024"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list