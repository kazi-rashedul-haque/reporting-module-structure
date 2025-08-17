# Title: Members_ConfigurationSwitching_BeforeSave_017

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
    - Report Name: EDGE_Members_ConfigurationSwitching_BeforeSave_017
    - Description: Edge case test for switching report configurations before saving
11. Click on "Next" to create the report
12. Select "Dual Axis" as the "Report Type"
13. Select "Members" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "X Axis" dropdown
16. Select "Total Members" from the "Y Axis Left (Bar)" dropdown
17. Select "Engaged Members" from the "Y Axis Right (Line)" dropdown
18. Switch to "Ideas" from the "Data Category" dropdown (verify X-axis and Y-axis reset)
19. Select "Stage" from the "X Axis" dropdown
20. Select "# of Ideas Submitted" from the "Y Axis Left (Bar)" dropdown
21. Select "# of Idea Views" from the "Y Axis Right (Line)" dropdown
22. Switch back to "Members" from the "Data Category" dropdown (verify X-axis and Y-axis reset again)
23. Select "Member Status" from the "X Axis" dropdown
24. Select "New Members" from the "Y Axis Left (Bar)" dropdown
25. Select "Total Logins" from the "Y Axis Right (Line)" dropdown
26. Verify "Save changes" button is not visible yet
27. Click on "Show Results" button
28. Verify "Save changes" button appears beside "Show Results" button
29. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
30. Click on "Save changes" button
31. Verify success message appears and disappears after a few seconds

# Expected Results:
- Configuration switching between data categories works correctly
- X-axis and Y-axis options reset appropriately when data category changes
- Final configuration (Members + Member Status + New Members + Total Logins) is saved
- Report saved successfully with name: "EDGE_Members_ConfigurationSwitching_BeforeSave_017"
- Report description: "Edge case test for switching report configurations before saving"
- Success message displayed
- Chart type: Dual axis chart displayed correctly with both bar charts and line charts
- X-Axis label: Shows member status data points
- Left Y-Axis label: Shows "New Members" for bar chart components
- Right Y-Axis label: Shows "Total Logins" for line chart components
- First column of table: "Dataset" containing both Y-axis values
- Subsequent columns: Based on Member Status X-axis selection
- Cell values: Match the corresponding dual axis chart data points when hovered
- Bar chart components displayed on left axis for "New Members"
- Line chart components displayed on right axis for "Total Logins"
- Configuration switching did not cause any UI errors or data corruption
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "EDGE_Members_ConfigurationSwitching_BeforeSave_017"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list