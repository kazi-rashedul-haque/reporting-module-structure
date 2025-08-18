# Unsaved Changes Dropdown - Does Not Appear Without Changes Test

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
9. Open an existing saved report from the list
10. Wait for the report to load completely
11. Verify report displays with saved configuration
12. Verify "Unsaved Changes" dropdown is not visible

## Expected Results:
- "Unsaved Changes" dropdown should not appear when opening existing saved report

## Test Data:
- Uses existing saved report from Reports list
- No new report creation required for this test

## Cleanup:
- No cleanup required as no new report is created
- Test uses existing saved reports only