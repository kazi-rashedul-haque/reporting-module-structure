# SMOKE_Ideas_Quarterly_CustomRange_004

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
    - Report Name: SMOKE_Ideas_Quarterly_CustomRange_004
    - Description: Smoke test for metric card with Custom Range time frame validation - Ideas category, Quarterly grouping
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown (should be selected by default)
14. Click on "Time Frame" button and select "Custom Range"
15. Verify date picker appears with "Start Date" and "End Date" fields
16. Set Start Date to 30 days ago from current date
17. Set End Date to current date
18. Verify valid date range is accepted
19. Click on "Data Grouping" dropdown and select "Quarterly"
20. Click on "Dataset" dropdown and select "# of Ideas Submitted"
21. Click on "Show Results" button
22. Verify "Save changes" button appears beside "Show Results" button
23. Verify "Unsaved Changes" dropdown appears at top-right corner
24. Verify metric card displays correctly with custom date range data
25. Verify table shows appropriate quarterly columns based on custom range
26. Click on "Save changes" button
27. Verify success message appears and disappears

## Expected Results:
- Report saved successfully with name: "SMOKE_Ideas_Quarterly_CustomRange_004"
- Custom Range time frame works correctly
- Date picker allows valid date range selection
- Start Date and End Date fields are functional
- Metric Card displays data for the specified custom range period
- Table columns adjust appropriately based on the custom date range
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

## Cleanup:
1. Navigate back to Reports list by clicking "Back" button
2. Search for the created report "SMOKE_Ideas_Quarterly_CustomRange_004"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option 
5. Confirm deletion
6. Verify report is removed from the list