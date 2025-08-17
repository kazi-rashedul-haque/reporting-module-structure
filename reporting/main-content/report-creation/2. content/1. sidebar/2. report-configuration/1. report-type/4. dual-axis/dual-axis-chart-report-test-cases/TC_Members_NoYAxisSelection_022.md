# Title: Members_NoYAxisSelection_022

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
    - Report Name: NEG_Members_NoYAxisSelection_022
    - Description: Negative test for attempting to create report without selecting Y-axis values
11. Click on "Next" to create the report
12. Select "Dual Axis" as the "Report Type"
13. Select "Members" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "X Axis" dropdown
16. Leave "Y Axis Left (Bar)" unselected (should show "Choose")
17. Leave "Y Axis Right (Line)" unselected (should show "Choose")
18. Verify "Show Results" button state
19. Attempt to click on "Show Results" button
20. Verify validation error appears for missing Y-axis selections
21. Verify no chart is generated without Y-axis values
22. Select "Total Members" from the "Y Axis Left (Bar)" dropdown
23. Verify "Show Results" button state changes
24. Attempt to click on "Show Results" button
25. Verify validation error appears for missing Y Axis Right (Line) selection
26. Select "Engaged Members" from the "Y Axis Right (Line)" dropdown
27. Verify "Show Results" button becomes fully enabled
28. Click on "Show Results" button
29. Verify "Save changes" button appears beside "Show Results" button
30. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
31. Click on "Save changes" button
32. Verify success message appears and disappears after a few seconds

# Expected Results:
- Cannot generate results without both Y-axis selections
- Validation error is displayed when trying to show results without Y Axis Left (Bar) selection
- Validation error is displayed when trying to show results without Y Axis Right (Line) selection
- "Show Results" button remains disabled or shows appropriate validation state
- After selecting first Y-axis value, still requires second Y-axis value for dual axis chart
- Both Y-axis values are required for dual axis chart generation
- Report saved successfully with name: "NEG_Members_NoYAxisSelection_022"
- Report description: "Negative test for attempting to create report without selecting Y-axis values"
- Success message displayed after both Y-axis values are selected
- Chart type: Dual axis chart displayed correctly with both bar charts and line charts
- X-Axis label: Shows quarterly data points
- Left Y-Axis label: Shows "Total Members" for bar chart components
- Right Y-Axis label: Shows "Engaged Members" for line chart components
- First column of table: "Dataset" containing both Y-axis values
- Subsequent columns: Based on quarterly selection
- Cell values: Match the corresponding dual axis chart data points when hovered
- Bar chart components displayed on left axis for "Total Members"
- Line chart components displayed on right axis for "Engaged Members"
- Y-axis validation works as expected for dual axis charts
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "NEG_Members_NoYAxisSelection_022"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list