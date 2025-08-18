# EDGE_MaxDatasets_AddDataset_004

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
    - Report Name: EDGE_MaxDatasets_AddDataset_004
    - Description: Edge case test for maximum datasets limit - testing Add Dataset boundary conditions
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "Data Grouping" dropdown and select "Quarterly"
16. Click on "Dataset" dropdown and select "# of Ideas Submitted"
17. Click on "Add Dataset" button
18. Verify second dataset dropdown appears
19. In the second dataset dropdown, select "# of Idea Views"
20. Attempt to click "Add Dataset" button again
21. Verify system behavior when trying to add a third dataset
22. Verify maximum of 2 datasets are allowed as per template specification
23. Click on "Show Results" button
24. Verify metric card displays with 2 datasets correctly
25. Verify table shows both datasets in separate rows
26. Click on "Save changes" button
27. Verify success message appears

## Expected Results:
- System allows adding exactly 2 datasets for metric card reports
- "Add Dataset" button becomes disabled or unavailable after adding second dataset
- Clear indication that maximum limit (2 datasets) has been reached
- Both datasets display correctly in the metric card table
- Each dataset shows as a separate row with quarterly breakdown
- No system errors when reaching maximum dataset limit
- Save functionality works normally with maximum datasets

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report "EDGE_MaxDatasets_AddDataset_004"