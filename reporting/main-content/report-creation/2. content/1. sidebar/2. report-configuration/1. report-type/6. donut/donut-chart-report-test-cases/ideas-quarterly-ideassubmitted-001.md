# Ideas_Quarterly_IdeasSubmitted_001

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
    - Report Name: DONUT_SMOKE_Ideas_Quarterly_IdeasSubmitted_001
    - Description: Smoke test for basic donut chart with Ideas data category, Quarterly grouping, and # of Ideas Submitted dataset
11. Click on "Next" to create the report
12. Select "Donut" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "Data Grouping" dropdown
16. Select "# of Ideas Submitted" from the "Dataset" dropdown
17. Verify "Save changes" button is not visible yet
18. Click on "Show Results" button
19. Verify "Save changes" button appears beside "Show Results" button
20. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
21. Verify donut chart displays with visual donut representation
22. Verify total value/count is prominently displayed in the center of the donut (expected: "26")
23. Verify legend appears on the right side with quarterly data grouping categories and color coding
24. Verify legend shows: Q3 2024, Q4 2024, Q1 2025, Q2 2025, Q3 2025
25. Verify chart segments are color-coded and proportional to data values
26. Verify data table below the chart shows detailed breakdown with exact values
27. Verify color coordination between chart segments and legend items
28. Verify chart and table data are synchronized and consistent
29. Verify data table structure:
    - First column: "Dataset" contains "# of Ideas Submitted"
    - Subsequent columns: Q3 2024, Q4 2024, Q1 2025, Q2 2025, Q3 2025
    - Data row shows: 0, 0, 0, 0, 26
30. Click on "Save changes" button
31. Verify success message appears: "DONUT_SMOKE_Ideas_Quarterly_IdeasSubmitted_001 has been successfully created."
32. Verify success message disappears after a few seconds

## Expected Results:
- Report saved successfully with name: "DONUT_SMOKE_Ideas_Quarterly_IdeasSubmitted_001"
- Report description: "Smoke test for basic donut chart with Ideas data category, Quarterly grouping, and # of Ideas Submitted dataset"
- Success message displayed and dismissed automatically
- Chart Type: Donut Chart displayed correctly with visual donut representation
- Donut chart shows total value/count prominently displayed in the center of the donut (value: "26")
- Legend displayed on the right side showing quarterly data grouping categories with color coding
- Interactive legend items that correspond to chart segments (Q3 2024, Q4 2024, Q1 2025, Q2 2025, Q3 2025)
- Chart segments are color-coded and proportional to data values
- Data table below the chart shows detailed breakdown with exact values for each quarter
- First column of table: "Dataset" contains "# of Ideas Submitted"
- Subsequent columns: Q3 2024, Q4 2024, Q1 2025, Q2 2025, Q3 2025 with values 0, 0, 0, 0, 26
- Chart and table data are synchronized and show consistent values
- Color coordination between chart segments and legend items
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

## Cleanup:
1. Navigate back to Reports list
2. Search for the created report "DONUT_SMOKE_Ideas_Quarterly_IdeasSubmitted_001"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option for the report
5. Confirm deletion
6. Verify report is removed from the list