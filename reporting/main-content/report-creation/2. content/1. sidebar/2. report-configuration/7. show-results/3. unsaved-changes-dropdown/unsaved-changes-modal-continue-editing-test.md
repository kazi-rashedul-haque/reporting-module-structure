# Unsaved Changes Warning Modal - Continue Editing Button Test

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
    - Report Name: Test Continue Editing Button
    - Description: Test to verify Continue Editing button functionality in warning modal
11. Click on "Next" to create the report
12. Select "Horizontal Bar" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown (should be selected by default)
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "X Axis" dropdown and select "Quarterly"
16. Click on "Y Axis" dropdown and select "# of Ideas Submitted"
17. Click on "Show Results" button
18. Wait for results to load
19. Verify "Unsaved Changes" dropdown appears in top-right corner
20. Click on "Back" button to attempt navigation
21. Verify warning modal appears with title "You have unsaved changes"
22. Click on "Continue Editing" button
23. Verify modal closes
24. Verify user remains on report creation page
25. Verify all report configuration remains unchanged
26. Verify "Unsaved Changes" dropdown is still visible in top-right corner

## Expected Results:
- "Continue Editing" button is clickable and functional
- Clicking "Continue Editing" closes the warning modal
- User remains on the current report creation page
- Report configuration remains exactly as it was before attempting navigation
- "Unsaved Changes" dropdown remains visible

## Test Data:
- Report Name: "Test Continue Editing Button"
- Report Description: "Test to verify Continue Editing button functionality in warning modal"

## Cleanup:
1. Click on "Unsaved Changes" dropdown
2. Click on "Save Changes" to save the report
3. Wait for save to complete
4. Navigate back to Reports list by clicking "Back" button
5. Search for the created report "Test Continue Editing Button"
6. Click on "More Actions" menu for the report
7. Click on "Delete" option
8. Confirm deletion
9. Verify report is removed from the list