# NEG_NoDataset_Selected_004

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
    - Report Name: NEG_NoDataset_Selected_004
    - Description: Negative test case for attempting to create metric card without selecting any dataset
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "Data Grouping" dropdown and select "Quarterly"
16. Leave "Dataset" dropdown unselected (should show "Choose")
17. Click on "Show Results" button without selecting any dataset
18. Verify system behavior when no dataset is selected
19. Observe validation messages or error handling
20. Check if "Show Results" button is disabled or shows error
21. Attempt to proceed with report generation without dataset selection

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