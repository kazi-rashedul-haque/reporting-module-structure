# Title: Members_WorkspaceGroup_TotalMembers_TotalLogins_EngagedMembers_NewMembers_013

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
    - Report Name: REG_Members_WorkspaceGroup_MaxDatasets_013
    - Description: Regression test for dual axis chart with Members using maximum datasets (2 per axis) and Workspace Group X-axis
11. Click on "Next" to create the report
12. Select "Dual Axis" as the "Report Type"
13. Select "Members" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Workspace Group" from the "X Axis" dropdown
16. Select "Total Members" from the "Y Axis Left (Bar)" dropdown
17. Click on "Add Dataset" button for Y Axis Left (Bar)
18. Select "Total Logins" from the new dropdown (different from already selected values)
19. Select "Engaged Members" from the "Y Axis Right (Line)" dropdown
20. Click on "Add Dataset" button for Y Axis Right (Line)
21. Select "New Members" from the new dropdown (different from already selected values)
22. Verify "Save changes" button is not visible yet
23. Click on "Show Results" button
24. Verify "Save changes" button appears beside "Show Results" button
25. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
26. Click on "Save changes" button
27. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "REG_Members_WorkspaceGroup_MaxDatasets_013"
- Report description: "Regression test for dual axis chart with Members using maximum datasets (2 per axis) and Workspace Group X-axis"
- Success message displayed
- Chart type: Dual axis chart displayed correctly with both bar charts and line charts
- X-Axis label: Shows workspace group data points
- Left Y-Axis label: Shows metrics for bar chart components ("Total Members" and "Total Logins")
- Right Y-Axis label: Shows metrics for line chart components ("Engaged Members" and "New Members")
- First column of table: "Dataset" containing all 4 Y-axis values
- Subsequent columns: Based on Workspace Group X-axis selection
- Cell values: Match the corresponding dual axis chart data points when hovered
- 2 Bar chart components displayed on left axis for the Left Y-axis datasets
- 2 Line chart components displayed on right axis for the Right Y-axis datasets
- Each dataset appears as separate components in the dual axis chart
- Each dataset gets its own row in the table (4 total rows)
- Maximum datasets limit (2 per axis) functionality works correctly
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "REG_Members_WorkspaceGroup_MaxDatasets_013"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list