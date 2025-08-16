# REG_Members_Last90Days_TotalVisits_011

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
    - Report Name: REG_Members_Last90Days_TotalVisits_011
    - Description: Regression test for metric card with Members category, Last 90 Days time frame, and Total Visits dataset
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Click on "Data Category" dropdown and select "Members"
14. Click on "Time Frame" button and select "Last 90 Days"
15. Click on "Data Grouping" dropdown and select "Weekly"
16. Click on "Dataset" dropdown and select "Total Visits"
17. Click on "Show Results" button
18. Verify metric card displays with weekly data breakdown for last 90 days
19. Verify table shows weekly columns for the 90-day period
20. Click on "Save changes" button
21. Verify success message appears

## Expected Results:
- Report created successfully with Last 90 Days time frame for Members category
- Weekly breakdown displays correctly for the 90-day period
- Total Visits dataset shows appropriate weekly values for last 90 days
- Table columns represent weekly time periods within the 90-day range
- Time frame functionality works correctly for 90-day periods

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report "REG_Members_Last90Days_TotalVisits_011"