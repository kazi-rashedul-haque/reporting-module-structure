# Members_Weekly_NewMembers_REG002

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
    - Report Name: TABLE_REG_Members_Weekly_NewMembers_002
    - Description: Regression test for table report with Members category, Weekly grouping, and New Members dataset
11. Click on "Next" to create the report
12. Select "Table" as the "Report Type"
13. Select "Members" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Weekly" from the "Data Grouping" dropdown
16. Select "New Members" from the "Dataset" dropdown
17. Click on "Show Results" button
18. Verify table displays with weekly columns (approximately 52 columns for weekly data over 365 days)
19. Verify first column shows "Dataset" with "New Members"
20. Verify weekly columns show week ranges or dates
21. Click on "Save changes" button
22. Verify success message appears: "TABLE_REG_Members_Weekly_NewMembers_002 has been successfully created."

## Expected Results:
- Report saved successfully with name: "TABLE_REG_Members_Weekly_NewMembers_002"
- Table displays with Weekly time grouping showing week-based columns
- First column: "Dataset" contains "New Members"
- Weekly columns display week ranges based on Last 365 Days timeframe
- Table may require horizontal scrolling due to multiple weekly columns
- Data values represent new member counts for each week
- Success message displayed and auto-dismisses
- Report URL indicates successful save

## Cleanup:
1. Navigate back to Reports list
2. Search for the created report "TABLE_REG_Members_Weekly_NewMembers_002"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option for the report
5. Confirm deletion
6. Verify report is removed from the list