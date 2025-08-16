# Ideas_Campaign_EngagementActions_REG003

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
    - Report Name: TABLE_REG_Ideas_Campaign_EngagementActions_003
    - Description: Regression test for table report with Ideas category, Campaign grouping (IDEA PROPERTIES), and Engagement Actions dataset
11. Click on "Next" to create the report
12. Select "Table" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Campaign" from the "Data Grouping" dropdown (under IDEA PROPERTIES section)
16. Select "Engagement Actions" from the "Dataset" dropdown
17. Click on "Show Results" button
18. Verify table displays with campaign-based columns (showing different campaign names)
19. Verify first column shows "Dataset" with "Engagement Actions"
20. Verify columns show campaign names instead of time periods
21. Click on "Save changes" button
22. Verify success message appears: "TABLE_REG_Ideas_Campaign_EngagementActions_003 has been successfully created."

## Expected Results:
- Report saved successfully with name: "TABLE_REG_Ideas_Campaign_EngagementActions_003"
- Table displays with Campaign grouping showing campaign-based columns instead of time-based columns
- First column: "Dataset" contains "Engagement Actions"
- Subsequent columns show campaign names (not time periods)
- Data values represent engagement action counts per campaign
- Table structure adapts to IDEA PROPERTIES grouping format
- Success message displayed and auto-dismisses
- Report URL indicates successful save

## Cleanup:
1. Navigate back to Reports list
2. Search for the created report "TABLE_REG_Ideas_Campaign_EngagementActions_003"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option for the report
5. Confirm deletion
6. Verify report is removed from the list