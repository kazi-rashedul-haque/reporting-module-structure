# Title: Ideas_TagsApplied_CommunityGroup_012

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
    - Report Name: REG_Ideas_TagsApplied_CommunityGroup_012
    - Description: Regression test for horizontal bar chart with Ideas data category, Tags Applied X-axis, and Community Group Y-axis
11. Click on "Next" to create the report
12. Select "Horizontal Bar" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Tags Applied" from the "X Axis" dropdown
16. Select "Community Group" from the "Y Axis" dropdown
17. Verify "Save changes" button is not visible yet
18. Click on "Show Results" button
19. Verify "Save changes" button appears beside "Show Results" button
20. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
21. Click on "Save changes" button
22. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "REG_Ideas_TagsApplied_CommunityGroup_012"
- Report description: "Regression test for horizontal bar chart with Ideas data category, Tags Applied X-axis, and Community Group Y-axis"
- Success message displayed
- Chart type: Horizontal bar chart displayed correctly with horizontal bars
- X-Axis label: Shows "Tags Applied" metric name in the top-right corner of the chart
- Y-Axis label: Shows different community group names
- First column of table: "Dataset" containing the X-axis value "Tags Applied"
- Subsequent columns: Different community group names based on data availability
- Cell values: Match the corresponding horizontal bar chart data points when hovered
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "REG_Ideas_TagsApplied_CommunityGroup_012"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list