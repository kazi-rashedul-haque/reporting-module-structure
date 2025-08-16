# Title: Ideas_InvalidCustomDateRange_023

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
    - Report Name: NEG_Ideas_InvalidCustomDateRange_023
    - Description: Negative test for invalid custom date ranges (end date before start date, future dates, very old dates)
11. Click on "Next" to create the report
12. Select "Dual Axis" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Click on "Time Frame" dropdown and select "Custom Range"
15. Verify date picker appears with "Start Date" and "End Date" fields
16. Test invalid range #1: End date before start date
    - Set Start Date to current date
    - Set End Date to yesterday's date
    - Verify validation error for invalid date range
17. Test invalid range #2: Future dates
    - Set Start Date to tomorrow's date
    - Set End Date to day after tomorrow
    - Verify validation error for future dates
18. Test invalid range #3: Very old dates (>5 years)
    - Set Start Date to 6 years ago
    - Set End Date to 5 years ago
    - Verify validation error or warning for very old dates
19. Test invalid range #4: Same start and end date
    - Set Start Date to current date
    - Set End Date to same current date
    - Verify validation behavior for same dates
20. Set valid date range: last 30 days
    - Set Start Date to 30 days ago
    - Set End Date to current date
    - Verify valid range is accepted
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
- Invalid date range validation is triggered appropriately:
  - End date before start date shows validation error
  - Future dates show validation error
  - Very old dates (>5 years) show validation error or warning
  - Same start and end date shows appropriate validation behavior
- User cannot proceed with invalid date ranges
- Valid date range (last 30 days) is accepted
- Custom Range date picker functionality works correctly
- Report saved successfully with name: "NEG_Ideas_InvalidCustomDateRange_023"
- Report description: "Negative test for invalid custom date ranges (end date before start date, future dates, very old dates)"
- Success message displayed after valid date range is set
- Chart type: Dual axis chart displayed correctly with both bar charts and line charts
- X-Axis label: Shows quarterly data points within the valid custom range
- Left Y-Axis label: Shows "# of Ideas Submitted" for bar chart components
- Right Y-Axis label: Shows "# of Idea Views" for line chart components
- First column of table: "Dataset" containing both Y-axis values
- Subsequent columns: Based on quarterly selection within custom date range
- Cell values: Match the corresponding dual axis chart data points when hovered
- Bar chart components displayed on left axis for "# of Ideas Submitted"
- Line chart components displayed on right axis for "# of Idea Views"
- Data reflects only the valid custom date range (last 30 days)
- Custom date range validation works as expected
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "NEG_Ideas_InvalidCustomDateRange_023"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list