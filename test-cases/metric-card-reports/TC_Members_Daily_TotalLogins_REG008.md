# REG_Members_Daily_TotalLogins_008

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
    - Report Name: REG_Members_Daily_TotalLogins_008
    - Description: Regression test for metric card with Members category, Daily grouping, and Total Logins dataset
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Click on "Data Category" dropdown and select "Members"
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "Data Grouping" dropdown and select "Daily"
16. Click on "Dataset" dropdown and select "Total Logins"
17. Click on "Show Results" button
18. Verify metric card displays with daily data breakdown
19. Verify table shows daily columns for the past 365 days
20. Click on "Save changes" button
21. Verify success message appears

## Expected Results:
- Report created successfully with Daily data grouping for Members category
- Daily breakdown displays correctly in metric card table
- Total Logins dataset shows appropriate daily values
- Table columns represent daily time periods within Last 365 Days range
- Report functionality works as expected for Members category with Daily grouping

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report "REG_Members_Daily_TotalLogins_008"