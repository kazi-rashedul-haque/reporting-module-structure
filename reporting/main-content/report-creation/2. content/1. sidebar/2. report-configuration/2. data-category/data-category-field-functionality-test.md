# Data Category Field - Functionality Test

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
    - Report Name: Test Data Category Field Functionality
    - Description: Test to verify Data Category field dropdown behavior
11. Click on "Next" to create the report
12. Select any report type to enable other fields
13. Locate the "Data Category" field section
14. Verify field is labeled "Data Category"
15. Click on the "Data Category" dropdown to open it
16. Verify dropdown opens and displays available options
17. Verify "Ideas" option is available in the dropdown
18. Verify "Members" option is available in the dropdown
19. Click on "Ideas" option
20. Verify "Ideas" is selected and dropdown closes
21. Click on the dropdown again to reopen it
22. Click on "Members" option
23. Verify "Members" is selected and dropdown closes
24. Verify the field updates to show "Members" as selected

## Expected Results:
- Field should be labeled "Data Category"
- Dropdown should contain exactly two options: "Ideas" and "Members"
- Selecting an option should close the dropdown and update the displayed value

## Test Data:
- Report Name: "Test Data Category Field Functionality"
- Report Description: "Test to verify Data Category field dropdown behavior"

## Cleanup:
1. Navigate back to Reports list by clicking "Back" button
2. Search for the created report "Test Data Category Field Functionality"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list