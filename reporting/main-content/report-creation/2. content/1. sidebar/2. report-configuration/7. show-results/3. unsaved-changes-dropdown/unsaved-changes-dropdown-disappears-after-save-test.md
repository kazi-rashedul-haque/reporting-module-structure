# Unsaved Changes Dropdown - Disappears After Save Test

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
    - Report Name: Test Dropdown Disappears After Save
    - Description: Test to verify dropdown disappears after successful save
11. Click on "Next" to create the report
12. Select "Table" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown (should be selected by default)
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "Data Grouping" dropdown and select "Quarterly"
16. Click on "Dataset" dropdown and select "# of Ideas Submitted"
17. Click on "Show Results" button
18. Wait for results to load
19. Verify "Unsaved Changes" dropdown appears in top-right corner
20. Verify dropdown is visible and accessible
21. Click on "Save Changes" button from sidebar (not dropdown)
22. Wait for save operation to complete
23. Verify success alert appears and disappears
24. Verify "Unsaved Changes" dropdown disappears from top-right corner
25. Verify navigation is now possible without warnings
26. Click on "Back" button
27. Verify no warning modal appears
28. Verify navigation proceeds normally

## Expected Results:
- "Unsaved Changes" dropdown appears after clicking "Show Results"
- After successful save operation, dropdown disappears completely
- Success alert confirms save operation
- "Unsaved Changes" dropdown is no longer visible
- Navigation away from page proceeds without warning modal
- No unsaved changes warnings appear after successful save

## Test Data:
- Report Name: "Test Dropdown Disappears After Save"
- Report Description: "Test to verify dropdown disappears after successful save"

## Cleanup:
1. Navigate back to Reports list
2. Search for the created report "Test Dropdown Disappears After Save"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list