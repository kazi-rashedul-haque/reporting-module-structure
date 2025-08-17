# Title: Ideas_MaxReportName_120Characters_014

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
    - Report Name: EDGE_Ideas_MaxReportName_120Characters_This_is_exactly_one_hundred_twenty_characters_long_test_report_name_014
    - Description: Edge case test for dual axis chart with maximum length report name (120 characters)
11. Verify the report name is exactly 120 characters long
12. Verify character counter shows "120/120"
13. Click on "Next" to create the report
14. Select "Dual Axis" as the "Report Type"
15. Select "Ideas" from the "Data Category" dropdown
16. Select "Last 365 Days" from the "Time Frame" dropdown
17. Select "Quarterly" from the "X Axis" dropdown
18. Select "# of Ideas Submitted" from the "Y Axis Left (Bar)" dropdown
19. Select "# of Idea Views" from the "Y Axis Right (Line)" dropdown
20. Verify "Save changes" button is not visible yet
21. Click on "Show Results" button
22. Verify "Save changes" button appears beside "Show Results" button
23. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
24. Click on "Save changes" button
25. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report name with exactly 120 characters is accepted
- Character counter displays "120/120" correctly
- Report saved successfully with name: "EDGE_Ideas_MaxReportName_120Characters_This_is_exactly_one_hundred_twenty_characters_long_test_report_name_014"
- Report description: "Edge case test for dual axis chart with maximum length report name (120 characters)"
- Success message displayed
- Chart type: Dual axis chart displayed correctly with both bar charts and line charts
- X-Axis label: Shows quarterly data points
- Left Y-Axis label: Shows "# of Ideas Submitted" for bar chart components
- Right Y-Axis label: Shows "# of Idea Views" for line chart components
- First column of table: "Dataset" containing both Y-axis values
- Subsequent columns: Based on quarterly selection
- Cell values: Match the corresponding dual axis chart data points when hovered
- Bar chart components displayed on left axis for "# of Ideas Submitted"
- Line chart components displayed on right axis for "# of Idea Views"
- Full report name is displayed correctly in the Reports list
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report using partial name "EDGE_Ideas_MaxReportName"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list