# Title: Ideas_EmptyReportName_019

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
    - Report Name: (leave empty)
    - Description: Negative test for empty report name validation
11. Verify report name field is empty
12. Attempt to click on "Next" button
13. Verify validation error appears
14. Verify "Next" button remains disabled or error prevents progression
15. Fill in a valid report name: NEG_Ideas_EmptyReportName_Fixed_019
16. Verify "Next" button becomes enabled
17. Click on "Next" to create the report
18. Select "Dual Axis" as the "Report Type"
19. Select "Ideas" from the "Data Category" dropdown
20. Select "Last 365 Days" from the "Time Frame" dropdown
21. Select "Quarterly" from the "X Axis" dropdown
22. Select "# of Ideas Submitted" from the "Y Axis Left (Bar)" dropdown
23. Select "# of Idea Views" from the "Y Axis Right (Line)" dropdown
24. Verify "Save changes" button is not visible yet
25. Click on "Show Results" button
26. Verify "Save changes" button appears beside "Show Results" button
27. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
28. Click on "Save changes" button
29. Verify success message appears and disappears after a few seconds

# Expected Results:
- Empty report name validation is triggered
- Error message is displayed for empty report name field
- "Next" button is disabled when report name is empty
- User cannot proceed to report configuration without valid report name
- After providing valid report name, validation passes
- Report saved successfully with name: "NEG_Ideas_EmptyReportName_Fixed_019"
- Report description: "Negative test for empty report name validation"
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
- Empty report name validation works as expected
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "NEG_Ideas_EmptyReportName_Fixed_019"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list