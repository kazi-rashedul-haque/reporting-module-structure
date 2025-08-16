# Title: Ideas_CampaignGroup_NetActivityScore_and_ModeratorActivity_017

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
    - Report Name: REG_Ideas_CampaignGroup_NetActivityScore_and_ModeratorActivity_017
    - Description: Regression test for bar chart with Add Dataset - Ideas data category, Campaign Group X-axis, Net Activity Score and Moderator Activity Count Y-axis
11. Click on "Next" to create the report
12. Select "Bar" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Campaign Group" from the "X Axis" dropdown
16. Select "Net Activity Score" from the "Y Axis" dropdown
17. Click on "Add Dataset" button
18. Select "Moderator Activity Count" from the new Y-axis dropdown (different from first Y-axis value)
19. Verify "Save changes" button is not visible yet
20. Click on "Show Results" button
21. Verify "Save changes" button appears beside "Show Results" button
22. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
23. Click on "Save changes" button
24. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "REG_Ideas_CampaignGroup_NetActivityScore_and_ModeratorActivity_017"
- Report description: "Regression test for bar chart with Add Dataset - Ideas data category, Campaign Group X-axis, Net Activity Score and Moderator Activity Count Y-axis"
- Success message displayed
- Chart type: Bar chart displayed correctly with two separate bar groups
- X-Axis label: Shows different campaign group names
- Y-Axis label: Shows both metric names "Net Activity Score" and "Moderator Activity Count" in the top-right corner of the chart
- First row of table: "Dataset" containing the first Y-axis value "Net Activity Score"
- Second row of table: "Dataset" containing the second Y-axis value "Moderator Activity Count"
- Subsequent columns: Different campaign group names based on data availability
- Cell values: Match the corresponding bar chart data points when hovered for both datasets
- Each dataset appears as a separate bar group in the chart
- Add Dataset functionality works correctly with maximum 1 additional dataset
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "REG_Ideas_CampaignGroup_NetActivityScore_and_ModeratorActivity_017"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list