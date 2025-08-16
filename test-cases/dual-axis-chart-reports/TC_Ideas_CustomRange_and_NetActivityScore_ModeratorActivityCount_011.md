# Title: Ideas_CustomRange_NetActivityScore_ModeratorActivityCount_011

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
    - Report Name: REG_Ideas_CustomRange_NetActivityScore_ModeratorActivityCount_011
    - Description: Regression test for dual axis chart with Custom Range time frame validation (last 30 days)
11. Click on "Next" to create the report
12. Select "Dual Axis" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Click on "Time Frame" dropdown and select "Custom Range"
15. Verify date picker appears with "Start Date" and "End Date" fields
16. Set Start Date to 30 days ago from current date
17. Set End Date to current date
18. Verify valid date range is accepted
19. Select "Quarterly" from the "X Axis" dropdown
20. Select "Net Activity Score" from the "Y Axis Left (Bar)" dropdown
21. Select "Moderator Activity Count" from the "Y Axis Right (Line)" dropdown
22. Verify "Save changes" button is not visible yet
23. Click on "Show Results" button
24. Verify "Save changes" button appears beside "Show Results" button
25. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
26. Click on "Save changes" button
27. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "REG_Ideas_CustomRange_NetActivityScore_ModeratorActivityCount_011"
- Report description: "Regression test for dual axis chart with Custom Range time frame validation (last 30 days)"
- Success message displayed
- Custom Range date picker functionality works correctly
- Valid date range (last 30 days) is accepted
- Chart type: Dual axis chart displayed correctly with both bar charts and line charts
- X-Axis label: Shows quarterly data points within the custom range
- Left Y-Axis label: Shows "Net Activity Score" for bar chart components
- Right Y-Axis label: Shows "Moderator Activity Count" for line chart components
- First column of table: "Dataset" containing both Y-axis values
- Subsequent columns: Based on quarterly selection within custom date range
- Cell values: Match the corresponding dual axis chart data points when hovered
- Bar chart components displayed on left axis for "Net Activity Score"
- Line chart components displayed on right axis for "Moderator Activity Count"
- Data reflects only the custom date range (last 30 days)
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "REG_Ideas_CustomRange_NetActivityScore_ModeratorActivityCount_011"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list