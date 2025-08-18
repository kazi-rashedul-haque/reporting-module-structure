# Title: Members_SwitchConfiguration_025

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
    - Report Name: EDGE_Members_SwitchConfiguration_025
    - Description: Edge case test for switching between report configurations before saving
11. Click on "Next" to create the report
12. Select "Line" as the "Report Type"
13. Select "Members" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "X Axis" dropdown
16. Select "Total Members" from the "Y Axis" dropdown
17. Click on "Show Results" button to generate initial chart
18. Change "Data Category" from "Members" to "Ideas"
19. Verify that X-axis and Y-axis options change accordingly
20. Select "# of Ideas Submitted" from the updated "Y Axis" dropdown
21. Change "X Axis" from "Quarterly" to "Campaign"
22. Change "Y Axis" from "# of Ideas Submitted" to "# of Idea Views"
23. Click on "Add Dataset" button
24. Select "Engagement Actions" from the new dropdown
25. Verify "Save changes" button is not visible yet
26. Click on "Show Results" button
27. Verify "Save changes" button appears beside "Show Results" button
28. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
29. Click on "Save changes" button
30. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "EDGE_Members_SwitchConfiguration_025"
- Report description: "Edge case test for switching between report configurations before saving"
- Configuration switching works correctly without errors
- X-axis and Y-axis options update properly when Data Category is changed
- Final configuration reflects the last selected options: Ideas data category, Campaign X-axis, # of Idea Views + Engagement Actions Y-axis
- Success message displayed
- Chart type: Line chart displayed correctly with two lines
- X-Axis label: Shows campaign data points
- Y-Axis label: Shows both "# of Idea Views" and "Engagement Actions" metric names in the top-right corner of the chart
- First row of table: "Dataset" containing "# of Idea Views"
- Second row of table: "Dataset" containing "Engagement Actions"
- Subsequent columns: Based on Campaign selection
- Cell values: Match the corresponding line chart data points when hovered
- Each dataset appears as a separate line in the chart with different colors
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "EDGE_Members_SwitchConfiguration_025"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list