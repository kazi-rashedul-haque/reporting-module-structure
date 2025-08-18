# Title: Ideas_CustomRange_SameDates_026

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
    - Report Name: EDGE_Ideas_CustomRange_SameDates_026
    - Description: Edge case test for Custom Range with same start and end date validation
11. Click on "Next" to create the report
12. Select "Line" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Custom Range" from the "Time Frame" dropdown
15. Verify date picker appears with "Start Date" and "End Date"
16. Set Start Date to current date
17. Set End Date to the same current date (same as start date)
18. Select "Quarterly" from the "X Axis" dropdown
19. Select "# of Ideas Submitted" from the "Y Axis" dropdown
20. Verify "Save changes" button is not visible yet
21. Click on "Show Results" button
22. Verify system handles same start and end date appropriately (may show validation error or process single-day range)
23. If validation allows, verify "Save changes" button appears beside "Show Results" button
24. If validation allows, verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
25. If validation allows, click on "Save changes" button
26. If validation allows, verify success message appears and disappears after a few seconds

# Expected Results:
- Report name: "EDGE_Ideas_CustomRange_SameDates_026"
- Report description: "Edge case test for Custom Range with same start and end date validation"
- System properly handles same start and end date scenario
- Either shows appropriate validation error message for invalid date range OR processes single-day date range correctly
- If validation allows single-day range:
  - Success message displayed
  - Chart type: Line chart displayed correctly
  - X-Axis label: Shows data points for the single date
  - Y-Axis label: Shows "# of Ideas Submitted" metric name in the top-right corner of the chart
  - First column of table: "Dataset" containing the Y-axis value "# of Ideas Submitted"
  - Subsequent columns: Based on the single date selected
  - Cell values: Match the corresponding line chart data points when hovered
  - "Save changes" button becomes disabled/hidden after successful save
  - "Unsaved Changes" indicator disappears from top-right corner
  - Report appears in the Reports list when navigating back
- If validation prevents single-day range:
  - Appropriate error message displayed
  - User is prompted to select a valid date range
  - System prevents proceeding without valid date range

# Cleanup:
1. If report was successfully created, navigate back to Reports list
2. Search for the created report "EDGE_Ideas_CustomRange_SameDates_026"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list