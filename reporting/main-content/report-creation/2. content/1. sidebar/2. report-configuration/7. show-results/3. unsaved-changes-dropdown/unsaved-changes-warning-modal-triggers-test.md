# Unsaved Changes Warning Modal - Triggers on Navigation Test

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
    - Report Name: Test Unsaved Changes Warning Modal
    - Description: Test to verify warning modal triggers on navigation with unsaved changes
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown (should be selected by default)
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "Data Grouping" dropdown and select "Quarterly"
16. Click on "Dataset" dropdown and select "# of Ideas Submitted"
17. Click on "Show Results" button
18. Wait for results to load
19. Verify "Unsaved Changes" dropdown appears in top-right corner
20. Click on "Back" button to attempt navigation
21. Verify warning modal appears
22. Verify modal title displays "You have unsaved changes"
23. Verify modal description displays "Click `Continue Editing` to keep editing or `Discard Changes` to abandon changes."
24. Verify modal contains "Continue Editing" button
25. Verify modal contains "Discard Changes" button

## Expected Results:
- Warning modal triggers when attempting to navigate away with unsaved changes
- Modal title displays exactly "You have unsaved changes"
- Modal description displays exactly "Click `Continue Editing` to keep editing or `Discard Changes` to abandon changes."
- Modal contains "Continue Editing" button
- Modal contains "Discard Changes" button

## Test Data:
- Report Name: "Test Unsaved Changes Warning Modal"
- Report Description: "Test to verify warning modal triggers on navigation with unsaved changes"

## Cleanup:
1. Click "Discard Changes" button in modal to proceed with navigation
2. Navigate back to Reports list
3. Search for the created report "Test Unsaved Changes Warning Modal"
4. Click on "More Actions" menu for the report
5. Click on "Delete" option
6. Confirm deletion
7. Verify report is removed from the list