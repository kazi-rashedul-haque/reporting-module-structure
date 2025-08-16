# Ideas_Quarterly_AddDataset_003

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
    - Report Name: DONUT_SMOKE_Ideas_Quarterly_AddDataset_003
    - Description: Smoke test for donut chart with Ideas category, Quarterly grouping, and Add Dataset functionality
11. Click on "Next" to create the report
12. Select "Donut" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "Data Grouping" dropdown
16. Select "# of Ideas Submitted" from the "Dataset" dropdown
17. Click on "Add Dataset" button
18. Verify second dataset dropdown appears
19. Select "# of Idea Views" from the second dataset dropdown
20. Verify "Save changes" button is not visible yet
21. Click on "Show Results" button
22. Verify "Save changes" button appears beside "Show Results" button
23. Verify "Unsaved Changes" dropdown appears at top-right corner
24. Verify donut chart displays with visual donut representation
25. Verify total value/count is prominently displayed in the center of the donut
26. Verify legend appears on the right side with quarterly data grouping categories and color coding
27. Verify chart segments are color-coded and proportional to data values
28. Verify data table below the chart shows detailed breakdown with exact values
29. Verify data table structure:
    - First column: "Dataset" 
    - First data row: "# of Ideas Submitted" with quarterly values
    - Second data row: "# of Idea Views" with quarterly values
    - Subsequent columns: Q3 2024, Q4 2024, Q1 2025, Q2 2025, Q3 2025
30. Verify both datasets are represented in the chart visualization
31. Verify color coordination between chart segments and legend items
32. Verify chart and table data are synchronized and consistent
33. Click on "Save changes" button
34. Verify success message appears: "DONUT_SMOKE_Ideas_Quarterly_AddDataset_003 has been successfully created."

## Expected Results:
- Report saved successfully with name: "DONUT_SMOKE_Ideas_Quarterly_AddDataset_003"
- Report description: "Smoke test for donut chart with Ideas category, Quarterly grouping, and Add Dataset functionality"
- Add Dataset functionality works correctly allowing maximum of 1 additional dataset
- Chart Type: Donut Chart displayed correctly with visual donut representation for multiple datasets
- Donut chart shows total value/count prominently displayed in the center
- Legend displayed on the right side showing quarterly data grouping categories with color coding
- Data table shows both datasets with their respective values:
  - "# of Ideas Submitted" with quarterly breakdown
  - "# of Idea Views" with quarterly breakdown
- Chart segments properly represent multiple datasets with appropriate color coding
- All visual elements maintain consistency and coordination
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

## Cleanup:
1. Navigate back to Reports list
2. Search for the created report "DONUT_SMOKE_Ideas_Quarterly_AddDataset_003"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option for the report
5. Confirm deletion
6. Verify report is removed from the list