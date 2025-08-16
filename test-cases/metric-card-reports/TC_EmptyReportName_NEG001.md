# NEG_EmptyReportName_001

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
10. Leave the report details fields as follows:
    - Report Name: (Leave completely empty)
    - Description: Negative test case for empty report name validation
11. Click on "Next" button
12. Verify system behavior when report name is empty
13. Observe validation messages or error handling
14. If validation prevents proceeding, verify error message clarity
15. If allowed to proceed, attempt to complete report creation:
    - Select "Metric Card" as the "Report Type"
    - Select default configurations
    - Click "Show Results"
    - Attempt to save
16. Verify system prevents saving or provides appropriate error handling

## Expected Results:
- System prevents report creation with empty report name
- Clear validation error message appears: "Report name is required" or similar
- "Next" button remains disabled or shows validation error
- User cannot proceed to report configuration without entering a name
- Error message is prominently displayed and user-friendly
- Field is highlighted or marked as invalid
- System maintains data integrity by preventing invalid report creation

## Cleanup:
- No cleanup required as report should not be created with empty name