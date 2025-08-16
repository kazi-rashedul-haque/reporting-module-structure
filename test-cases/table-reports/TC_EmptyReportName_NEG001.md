# EmptyReportName_NEG001

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
    - Report Name: [Leave empty]
    - Description: Negative test case for empty report name validation
11. Verify character count shows "0/120"
12. Click on "Next" button
13. Verify system behavior when report name is empty
14. Observe validation messages or restrictions

## Expected Results:
- System prevents creation of report with empty name
- "Next" button is disabled when report name is empty OR
- Clear validation error message appears: "Report name is required" or similar
- System highlights the Report Name field as required
- User cannot proceed to report configuration without entering a report name
- Form validation prevents submission with empty required field
- Error message is prominently displayed and user-friendly

## Cleanup:
- No cleanup required as report should not be created with empty name