# EDGE_CustomRange_SameDate_005

## Pre-Condition: User has access to Reporting app with proper permissions

## Test Steps:
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
    - Report Name: EDGE_CustomRange_SameDate_005
    - Description: Edge case test for Custom Range with same start and end date
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Click on "Time Frame" button and select "Custom Range"
15. Verify date picker appears with "Start Date" and "End Date" fields
16. Set Start Date to today's date
17. Set End Date to the same date as Start Date (same day)
18. Verify system behavior with identical start and end dates
19. Click on "Data Grouping" dropdown and select "Daily"
20. Click on "Dataset" dropdown and select "# of Ideas Submitted"
21. Click on "Show Results" button
22. Verify metric card behavior with single-day date range
23. Verify table shows appropriate column(s) for single day
24. Click on "Save changes" button (if results are generated)
25. Verify system handling of edge case date range

## Expected Results:
- System appropriately handles same start and end date in Custom Range
- Either accepts single-day range or provides clear validation message
- If accepted, metric card displays data for the single day specified
- Table shows appropriate column structure for single-day period
- No system errors or crashes with edge case date input
- Clear user feedback about the date range selection
- Data grouping adjusts appropriately for single-day period

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report "EDGE_CustomRange_SameDate_005" (if successfully created)