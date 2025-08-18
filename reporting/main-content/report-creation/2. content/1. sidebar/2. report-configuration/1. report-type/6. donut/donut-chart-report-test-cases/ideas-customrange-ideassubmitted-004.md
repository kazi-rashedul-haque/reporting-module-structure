# Ideas_CustomRange_IdeasSubmitted_004

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
    - Report Name: DONUT_SMOKE_Ideas_CustomRange_IdeasSubmitted_004
    - Description: Smoke test for donut chart with Ideas category, Custom Range time frame, and # of Ideas Submitted dataset
11. Click on "Next" to create the report
12. Select "Donut" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Select "Custom Range" from the "Time Frame" dropdown
15. Verify date picker appears with "Start Date" and "End Date" fields
16. Set a valid custom range (e.g., last 30 days):
    - Start Date: 30 days ago from today
    - End Date: Today's date
17. Select "Quarterly" from the "Data Grouping" dropdown
18. Select "# of Ideas Submitted" from the "Dataset" dropdown
19. Verify "Save changes" button is not visible yet
20. Click on "Show Results" button
21. Verify "Save changes" button appears beside "Show Results" button
22. Verify "Unsaved Changes" dropdown appears at top-right corner
23. Verify donut chart displays with visual donut representation
24. Verify total value/count is prominently displayed in the center of the donut
25. Verify legend appears on the right side with data grouping categories appropriate for custom range
26. Verify chart segments are color-coded and proportional to data values
27. Verify data table below the chart shows detailed breakdown with exact values
28. Verify data table structure reflects the custom date range selected
29. Verify color coordination between chart segments and legend items
30. Verify chart and table data are synchronized and consistent for the custom range
31. Click on "Save changes" button
32. Verify success message appears: "DONUT_SMOKE_Ideas_CustomRange_IdeasSubmitted_004 has been successfully created."

## Expected Results:
- Report saved successfully with name: "DONUT_SMOKE_Ideas_CustomRange_IdeasSubmitted_004"
- Report description: "Smoke test for donut chart with Ideas category, Custom Range time frame, and # of Ideas Submitted dataset"
- Custom Range time frame functionality works correctly
- Date picker appears and accepts valid date range input
- Chart Type: Donut Chart displayed correctly with visual donut representation
- Donut chart shows total value/count prominently displayed in the center
- Legend displayed on the right side showing data appropriate for the selected custom range
- Data table shows data filtered to the specified custom date range
- Chart segments properly represent data within the custom time frame
- All visual elements maintain consistency and coordination
- Data reflects only the custom date range specified (not full year data)
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

## Cleanup:
1. Navigate back to Reports list
2. Search for the created report "DONUT_SMOKE_Ideas_CustomRange_IdeasSubmitted_004"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option for the report
5. Confirm deletion
6. Verify report is removed from the list