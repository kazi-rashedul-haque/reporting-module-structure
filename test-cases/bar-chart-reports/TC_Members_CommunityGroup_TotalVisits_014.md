# Title: Members_CommunityGroup_TotalVisits_014

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
    - Report Name: REG_Members_CommunityGroup_TotalVisits_014
    - Description: Regression test for bar chart with Members data category, Community Group X-axis, and Total Visits Y-axis
11. Click on "Next" to create the report
12. Select "Bar" as the "Report Type"
13. Select "Members" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Community Group" from the "X Axis" dropdown
16. Select "Total Visits" from the "Y Axis" dropdown
17. Verify "Save changes" button is not visible yet
18. Click on "Show Results" button
19. Verify "Save changes" button appears beside "Show Results" button
20. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
21. Click on "Save changes" button
22. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "REG_Members_CommunityGroup_TotalVisits_014"
- Report description: "Regression test for bar chart with Members data category, Community Group X-axis, and Total Visits Y-axis"
- Success message displayed
- Chart type: Bar chart displayed correctly
- X-Axis label: Shows different community group names
- Y-Axis label: Shows "Total Visits" metric name in the top-right corner of the chart
- First column of table: "Dataset" containing the Y-axis value "Total Visits"
- Subsequent columns: Different community group names based on data availability
- Cell values: Match the corresponding bar chart data points when hovered
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "REG_Members_CommunityGroup_TotalVisits_014"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list