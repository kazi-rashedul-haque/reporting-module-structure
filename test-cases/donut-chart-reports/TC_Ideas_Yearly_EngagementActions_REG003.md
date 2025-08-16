# IDEAS_Yearly_EngagementActions_REG003

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
    - Report Name: DONUT_REG_Ideas_Yearly_EngagementActions_003
    - Description: Regression test for donut chart with Ideas category, Yearly grouping, and Engagement Actions dataset
11. Click on "Next" to create the report
12. Select "Donut" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Yearly" from the "Data Grouping" dropdown
16. Select "Engagement Actions" from the "Dataset" dropdown
17. Click on "Show Results" button
18. Verify donut chart displays with visual donut representation
19. Verify legend shows yearly data grouping
20. Verify data table shows yearly breakdown
21. Verify chart segments are proportional to yearly engagement action counts
22. Click on "Save changes" button
23. Verify success message appears

## Expected Results:
- Report saved successfully with name: "DONUT_REG_Ideas_Yearly_EngagementActions_003"
- Chart Type: Donut Chart displayed correctly with yearly granularity
- Legend shows yearly periods (likely current year data)
- Data table shows yearly breakdown with "Engagement Actions" dataset
- Chart properly aggregates data into yearly periods
- All visual elements maintain consistency with yearly grouping

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report "DONUT_REG_Ideas_Yearly_EngagementActions_003"
3. Confirm deletion