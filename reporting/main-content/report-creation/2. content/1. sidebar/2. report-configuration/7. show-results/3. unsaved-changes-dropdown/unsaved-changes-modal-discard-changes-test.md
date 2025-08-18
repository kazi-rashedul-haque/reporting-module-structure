# Unsaved Changes Warning Modal - Discard Changes Button Test

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
    - Report Name: Test Discard Changes Button
    - Description: Test to verify Discard Changes button functionality in warning modal
11. Click on "Next" to create the report
12. Select "Dual Axis" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown (should be selected by default)
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "X Axis" dropdown and select "Quarterly"
16. Click on "Y Axis" dropdown and select "# of Ideas Submitted"
17. Click on "Y Axis" dropdown and select "# of Idea Views" as second dataset
18. Click on "Show Results" button
19. Wait for results to load
20. Verify "Unsaved Changes" dropdown appears in top-right corner
21. Note the current report configuration and data displayed
22. Click on "Back" button to attempt navigation
23. Verify warning modal appears with title "You have unsaved changes"
24. Click on "Discard Changes" button
25. Verify modal closes
27. Verify user is taken back to Reports list page
29. Navigate back to the report to verify previous state is retained

## Expected Results:
- "Discard Changes" button is clickable and functional
- Clicking "Discard Changes" closes the warning modal
- Navigation proceeds successfully after clicking "Discard Changes"
- User is taken to the intended destination (Reports list)
- When returning to the report, previous report state is retained (before the unsaved changes)

## Test Data:
- Report Name: "Test Discard Changes Button"
- Report Description: "Test to verify Discard Changes button functionality in warning modal"

## Cleanup:
1. Navigate back to Reports list (should already be there after discard)
2. Search for the created report "Test Discard Changes Button"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list