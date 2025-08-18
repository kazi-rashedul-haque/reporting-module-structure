# Title: Ideas_MaxDatasets_FourAxisValues_018

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
    - Report Name: EDGE_Ideas_MaxDatasets_FourAxisValues_018
    - Description: Edge case test for maximum datasets - 4 total Y-axis values (2 Left Bar + 2 Right Line)
11. Click on "Next" to create the report
12. Select "Dual Axis" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "X Axis" dropdown
16. Select "# of Ideas Submitted" from the "Y Axis Left (Bar)" dropdown
17. Click on "Add Dataset" button for Y Axis Left (Bar)
18. Select "# of Idea Views" from the new dropdown (different from already selected)
19. Verify maximum datasets reached for Left axis (should show "Max 2 datasets")
20. Select "# of Idea Votes" from the "Y Axis Right (Line)" dropdown
21. Click on "Add Dataset" button for Y Axis Right (Line)
22. Select "Engagement Actions" from the new dropdown (different from already selected)
23. Verify maximum datasets reached for Right axis (should show "Max 2 datasets")
24. Verify no additional "Add Dataset" buttons are available (total of 4 Y-axis values)
25. Verify "Save changes" button is not visible yet
26. Click on "Show Results" button
27. Verify "Save changes" button appears beside "Show Results" button
28. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
29. Click on "Save changes" button
30. Verify success message appears and disappears after a few seconds

# Expected Results:
- Maximum 4 Y-axis values are accepted (2 per axis)
- "Add Dataset" functionality correctly limits to 2 datasets per axis
- No additional "Add Dataset" buttons appear after maximum is reached
- Report saved successfully with name: "EDGE_Ideas_MaxDatasets_FourAxisValues_018"
- Report description: "Edge case test for maximum datasets - 4 total Y-axis values (2 Left Bar + 2 Right Line)"
- Success message displayed
- Chart type: Dual axis chart displayed correctly with both bar charts and line charts
- X-Axis label: Shows quarterly data points
- Left Y-Axis label: Shows metrics for bar chart components ("# of Ideas Submitted" and "# of Idea Views")
- Right Y-Axis label: Shows metrics for line chart components ("# of Idea Votes" and "Engagement Actions")
- First column of table: "Dataset" containing all 4 Y-axis values
- Subsequent columns: Based on quarterly selection
- Cell values: Match the corresponding dual axis chart data points when hovered
- 2 Bar chart components displayed on left axis for Left Y-axis datasets
- 2 Line chart components displayed on right axis for Right Y-axis datasets
- Each dataset appears as separate components in the dual axis chart
- Each dataset gets its own row in the table (4 total rows)
- Maximum datasets limit enforced correctly throughout the flow
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "EDGE_Ideas_MaxDatasets_FourAxisValues_018"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list