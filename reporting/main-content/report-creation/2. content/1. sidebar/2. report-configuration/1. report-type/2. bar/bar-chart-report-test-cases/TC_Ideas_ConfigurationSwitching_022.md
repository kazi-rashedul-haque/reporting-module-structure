# Title: Ideas_ConfigurationSwitching_022

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
    - Report Name: EDGE_ConfigurationSwitching_022
    - Description: Edge case test for switching between different report configurations before saving
11. Click on "Next" to create the report
12. Select "Bar" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "X Axis" dropdown
16. Select "# of Ideas Submitted" from the "Y Axis" dropdown
17. Switch to "Members" from the "Data Category" dropdown
18. Verify X-axis and Y-axis options update appropriately for Members category
19. Select "Member Status" from the "X Axis" dropdown
20. Select "Total Members" from the "Y Axis" dropdown
21. Switch back to "Ideas" from the "Data Category" dropdown
22. Verify X-axis and Y-axis reset or update appropriately
23. Select "Stage" from the "X Axis" dropdown
24. Select "Engagement Actions" from the "Y Axis" dropdown
25. Verify "Save changes" button is not visible yet
26. Click on "Show Results" button
27. Verify "Save changes" button appears beside "Show Results" button
28. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
29. Click on "Save changes" button
30. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "EDGE_ConfigurationSwitching_022"
- Report description: "Edge case test for switching between different report configurations before saving"
- Success message displayed
- Configuration switching between data categories works correctly
- X-axis and Y-axis options update dynamically based on data category selection
- Final configuration (Ideas + Stage + Engagement Actions) is properly saved
- Chart type: Bar chart displayed correctly
- X-Axis label: Shows different idea stages
- Y-Axis label: Shows "Engagement Actions" metric name in the top-right corner of the chart
- First column of table: "Dataset" containing the Y-axis value "Engagement Actions"
- Subsequent columns: Different stage names based on data availability
- Cell values: Match the corresponding bar chart data points when hovered
- Previous configurations are overridden by final selection
- System handles multiple configuration changes without errors
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "EDGE_ConfigurationSwitching_022"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list