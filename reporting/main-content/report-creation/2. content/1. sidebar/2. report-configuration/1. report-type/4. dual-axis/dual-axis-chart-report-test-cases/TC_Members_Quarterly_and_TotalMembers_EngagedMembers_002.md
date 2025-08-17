# Title: Members_Quarterly_TotalMembers_EngagedMembers_002

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
    - Report Name: SMOKE_Members_Quarterly_TotalMembers_EngagedMembers_002
    - Description: Smoke test for basic dual axis chart with Members data category, Quarterly X-axis, Total Members on left axis (Bar) and Engaged Members on right axis (Line)
11. Click on "Next" to create the report
12. Select "Dual Axis" as the "Report Type"
13. Select "Members" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "X Axis" dropdown
16. Select "Total Members" from the "Y Axis Left (Bar)" dropdown
17. Select "Engaged Members" from the "Y Axis Right (Line)" dropdown
18. Verify "Save changes" button is not visible yet
19. Click on "Show Results" button
20. Verify "Save changes" button appears beside "Show Results" button
21. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
22. Click on "Save changes" button
23. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "SMOKE_Members_Quarterly_TotalMembers_EngagedMembers_002"
- Report description: "Smoke test for basic dual axis chart with Members data category, Quarterly X-axis, Total Members on left axis (Bar) and Engaged Members on right axis (Line)"
- Success message displayed
- Chart type: Dual axis chart displayed correctly with both bar charts and line charts
- X-Axis label: Shows quarterly data points (e.g., Q1 2024, Q2 2024, Q3 2024, Q4 2024)
- Left Y-Axis label: Shows "Total Members" for bar chart components
- Right Y-Axis label: Shows "Engaged Members" for line chart components
- First column of table: "Dataset" containing both Y-axis values
- Subsequent columns: Based on quarterly selection (Q1 2024, Q2 2024, Q3 2024, Q4 2024)
- Cell values: Match the corresponding dual axis chart data points when hovered
- Bar chart components displayed on left axis for "Total Members"
- Line chart components displayed on right axis for "Engaged Members"
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "SMOKE_Members_Quarterly_TotalMembers_EngagedMembers_002"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list