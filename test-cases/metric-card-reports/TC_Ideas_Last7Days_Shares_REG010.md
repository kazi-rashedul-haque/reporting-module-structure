# REG_Ideas_Last7Days_Shares_010

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
    - Report Name: REG_Ideas_Last7Days_Shares_010
    - Description: Regression test for metric card with Ideas category, Last 7 Days time frame, and # of Shares dataset
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Click on "Time Frame" button and select "Last 7 Days"
15. Click on "Data Grouping" dropdown and select "Daily"
16. Click on "Dataset" dropdown and select "# of Shares"
17. Click on "Show Results" button
18. Verify metric card displays with daily data breakdown for last 7 days
19. Verify table shows 7 daily columns for the recent week
20. Click on "Save changes" button
21. Verify success message appears

## Expected Results:
- Report created successfully with Last 7 Days time frame for Ideas category
- Daily breakdown displays correctly for the recent 7-day period
- # of Shares dataset shows appropriate daily values for last 7 days
- Table columns represent the last 7 daily time periods
- Time frame functionality works correctly for short periods

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report "REG_Ideas_Last7Days_Shares_010"