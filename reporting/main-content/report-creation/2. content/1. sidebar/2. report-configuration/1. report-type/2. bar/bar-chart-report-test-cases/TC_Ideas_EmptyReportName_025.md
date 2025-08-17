# Title: Ideas_EmptyReportName_025

# Pre-Condition: User has access to Reporting app with proper permissions

# Test Steps:
1. Open the browser and navigate to: https://reporting.t1.ideascale.dev
2. Accept cookies if prompted
3. Log in with the following credentials:
   - Email: superuser@ideascale.me
   - Password: brewski01
4. Click on the "Apps" button in the header
5. Click on the "Reporting" app
6. Wait for the Reporting app to load
7. Click on "Reports" in the left sidebar
8. Wait for the Reports page to load
9. Click on "Create Report" button
10. Fill in the report details:
    - Report Name: [Leave completely empty]
    - Description: Negative test for empty report name validation with bar chart
11. Attempt to click on "Next" button
12. Verify that validation error appears for empty report name
13. Verify that "Next" button is disabled or validation prevents proceeding
14. Verify appropriate error message is displayed indicating report name is required
15. Verify character counter shows 0/120
16. Verify required field indicator (*) is visible next to Report Name field

# Expected Results:
- Report creation is prevented when report name is left empty
- Validation error message appears indicating that report name is required
- "Next" button is disabled or non-functional when report name is empty
- Error message clearly states "Report Name is required" or similar validation message
- User cannot proceed to report configuration without providing a report name
- Character counter shows 0/120
- Required field indicator (*) is visible next to Report Name field
- Form validation prevents submission until report name is provided
- No navigation to report configuration occurs
- User remains on the Create Report dialog
- System maintains data integrity by preventing incomplete report creation

# Cleanup:
1. Fill in a valid report name to clear the validation error
2. Click "Cancel" button to close the Create Report dialog
3. Verify that no incomplete report is created in the system