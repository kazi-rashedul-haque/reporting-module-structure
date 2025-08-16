# SMOKE_Members_Monthly_TotalMembers_005

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
    - Report Name: SMOKE_Members_Monthly_TotalMembers_005
    - Description: Smoke test for metric card with Members data category, Monthly grouping variation
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Click on "Data Category" dropdown and select "Members"
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "Data Grouping" dropdown and select "Monthly"
16. Click on "Dataset" dropdown and select "Total Members"
17. Click on "Show Results" button
18. Verify "Save changes" button appears beside "Show Results" button
19. Verify "Unsaved Changes" dropdown appears at top-right corner
20. Verify metric card displays correctly with total number and percentage change
21. Verify table shows monthly columns (based on Last 365 Days period)
22. Verify first row shows "Total Members" with monthly values
23. Click on "Save changes" button
24. Verify success message appears and disappears

## Expected Results:
- Report saved successfully with name: "SMOKE_Members_Monthly_TotalMembers_005"
- Monthly data grouping works correctly for Members category
- Metric Card displayed correctly; there is no chart for this type of report
- Table shows monthly breakdown instead of quarterly
- First column of table: "Dataset" contains the Dataset value(s)
- Monthly columns display appropriately for the 365-day period
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

## Cleanup:
1. Navigate back to Reports list by clicking "Back" button
2. Search for the created report "SMOKE_Members_Monthly_TotalMembers_005"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option 
5. Confirm deletion
6. Verify report is removed from the list