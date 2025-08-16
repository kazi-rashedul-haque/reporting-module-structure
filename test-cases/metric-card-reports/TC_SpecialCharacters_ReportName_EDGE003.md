# EDGE_SpecialCharacters_ReportName_003

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
    - Report Name: "Test!@#$%^&*()_+-=[]{}|;':\",./<>?`~Report"
    - Description: Edge case test for special characters in report name and description fields
11. Click on "Next" to create the report
12. Verify report creation behavior with special characters in name
13. Select "Metric Card" as the "Report Type"
14. Verify "Ideas" is selected from the "Data Category" dropdown
15. Click on "Time Frame" button and select "Last 365 Days"
16. Click on "Data Grouping" dropdown and select "Quarterly"
17. Click on "Dataset" dropdown and select "# of Ideas Submitted"
18. Click on "Show Results" button
19. Verify metric card displays correctly
20. Click on "Save changes" button
21. Verify success message behavior with special characters

## Expected Results:
- System handles special characters appropriately in report name
- Special characters are either accepted or properly validated with clear error messages
- If accepted, report name displays correctly with special characters
- Metric card functionality works normally regardless of special characters in name
- No system errors or crashes occur due to special character input
- Report appears correctly in Reports list with special characters handled appropriately

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report (if successfully created)