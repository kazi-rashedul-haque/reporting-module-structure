# IDEAS_IdeaProperties_Campaign_REG005

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
    - Report Name: DONUT_REG_Ideas_Campaign_IdeasSubmitted_005
    - Description: Regression test for donut chart with Ideas category, Campaign grouping (IDEA PROPERTIES), and # of Ideas Submitted dataset
11. Click on "Next" to create the report
12. Select "Donut" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Campaign" from the "Data Grouping" dropdown (IDEA PROPERTIES section)
16. Select "# of Ideas Submitted" from the "Dataset" dropdown
17. Click on "Show Results" button
18. Verify donut chart displays with visual donut representation
19. Verify legend shows campaign-based data grouping
20. Verify data table shows breakdown by different campaigns
21. Verify chart segments represent different campaigns proportionally
22. Click on "Save changes" button
23. Verify success message appears

## Expected Results:
- Report saved successfully with name: "DONUT_REG_Ideas_Campaign_IdeasSubmitted_005"
- Chart Type: Donut Chart displayed correctly with campaign-based grouping
- Legend shows different campaigns as grouping categories
- Data table shows breakdown by campaign names with idea submission counts
- Chart properly displays IDEA PROPERTIES grouping (non-time based)
- Each campaign appears as separate segment in donut chart

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report "DONUT_REG_Ideas_Campaign_IdeasSubmitted_005"
3. Confirm deletion