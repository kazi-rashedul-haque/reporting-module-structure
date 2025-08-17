# Title: Members_CustomRange_VeryOldDates_027

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
    - Report Name: EDGE_Members_CustomRange_VeryOldDates_027
    - Description: Edge case test for Custom Range with very old dates (>5 years ago) validation
11. Click on "Next" to create the report
12. Select "Line" as the "Report Type"
13. Select "Members" from the "Data Category" dropdown
14. Select "Custom Range" from the "Time Frame" dropdown
15. Verify date picker appears with "Start Date" and "End Date"
16. Set Start Date to a date more than 5 years ago (e.g., January 1, 2018)
17. Set End Date to a date more than 5 years ago but after start date (e.g., December 31, 2018)
18. Select "Quarterly" from the "X Axis" dropdown
19. Select "Total Members" from the "Y Axis" dropdown
20. Verify "Save changes" button is not visible yet
21. Click on "Show Results" button
22. Verify system handles very old date range appropriately (may show validation error or process with limited/no data)
23. If validation allows, verify "Save changes" button appears beside "Show Results" button
24. If validation allows, verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
25. If validation allows, click on "Save changes" button
26. If validation allows, verify success message appears and disappears after a few seconds

# Expected Results:
- Report name: "EDGE_Members_CustomRange_VeryOldDates_027"
- Report description: "Edge case test for Custom Range with very old dates (>5 years ago) validation"
- System properly handles very old date range scenario
- Either shows appropriate validation error message for dates beyond supported range OR processes old date range correctly (possibly with no data)
- If validation allows old date range:
  - Success message displayed
  - Chart type: Line chart displayed correctly (may show empty chart if no data exists for that period)
  - X-Axis label: Shows quarterly data points for the old date range
  - Y-Axis label: Shows "Total Members" metric name in the top-right corner of the chart
  - First column of table: "Dataset" containing the Y-axis value "Total Members"
  - Subsequent columns: Based on the old date range selected (Q1 2018, Q2 2018, Q3 2018, Q4 2018)
  - Cell values: Match the corresponding line chart data points when hovered (may be 0 or empty if no data)
  - "Save changes" button becomes disabled/hidden after successful save
  - "Unsaved Changes" indicator disappears from top-right corner
  - Report appears in the Reports list when navigating back
- If validation prevents old date range:
  - Appropriate error message displayed about date range limitations
  - User is prompted to select a supported date range
  - System prevents proceeding without valid date range

# Cleanup:
1. If report was successfully created, navigate back to Reports list
2. Search for the created report "EDGE_Members_CustomRange_VeryOldDates_027"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list