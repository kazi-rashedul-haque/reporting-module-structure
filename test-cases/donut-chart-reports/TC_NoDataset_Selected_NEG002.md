# NoDataset_Selected_NEG002

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
    - Report Name: DONUT_NEG_NoDataset_Selected_002
    - Description: Negative test case for attempting to create donut chart without selecting any dataset
11. Click on "Next" to create the report
12. Select "Donut" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "Data Grouping" dropdown
16. Leave "Dataset" dropdown unselected (should show "Choose")
17. Click on "Show Results" button without selecting any dataset
18. Verify system behavior when no dataset is selected
19. Observe validation messages or error handling

## Expected Results:
- System prevents report generation without dataset selection
- "Show Results" button is disabled when no dataset is selected OR
- Clear validation error message appears: "Please select a dataset" or similar
- System highlights the Dataset field as required
- User cannot proceed to view results without selecting at least one dataset
- Error message is prominently displayed and user-friendly
- System maintains data integrity by preventing incomplete report configuration

## Cleanup:
- No cleanup required as report should not be created without dataset selection