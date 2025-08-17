# REG_Ideas_Quarterly_SelectedIdeas_005

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
    - Report Name: REG_Ideas_Quarterly_SelectedIdeas_005
    - Description: Regression test for metric card with Ideas category, Quarterly grouping, and Selected Ideas dataset
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "Data Grouping" dropdown and select "Quarterly"
16. Click on "Dataset" dropdown and select "Selected Ideas"
17. Click on "Show Results" button
18. Verify metric card displays with quarterly data breakdown
19. Verify table shows quarterly columns (Q3 2024, Q4 2024, Q1 2025, Q2 2025, Q3 2025)
20. Click on "Save changes" button
21. Verify success message appears

## Expected Results:
- Report created successfully with Quarterly data grouping for Ideas category
- Quarterly breakdown displays correctly in metric card table
- Selected Ideas dataset shows appropriate quarterly values
- Table columns represent quarterly time periods (Q3 2024, Q4 2024, Q1 2025, Q2 2025, Q3 2025)
- Report functionality works as expected for Selected Ideas dataset

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report "REG_Ideas_Quarterly_SelectedIdeas_005"