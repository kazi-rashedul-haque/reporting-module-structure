# NEG_InvalidDateRange_CustomRange_005

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
    - Report Name: NEG_InvalidDateRange_CustomRange_005
    - Description: Negative test case for invalid date ranges in Custom Range time frame
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Click on "Time Frame" button and select "Custom Range"
15. Verify date picker appears with "Start Date" and "End Date" fields
16. Test invalid date range scenarios:
    a. Set End Date to a date BEFORE Start Date (e.g., Start: 2025-08-01, End: 2025-07-01)
    b. Set Start Date to a future date (e.g., next year)
    c. Set End Date to a future date beyond today
    d. Set Start Date to a very old date (e.g., >5 years ago)
17. For each invalid scenario, attempt to proceed with:
    - Data Grouping: "Quarterly"
    - Dataset: "# of Ideas Submitted"
18. Click on "Show Results" button
19. Verify system behavior with each invalid date range
20. Observe validation messages and error handling

## Expected Results:
- System prevents report generation with invalid date ranges
- Clear validation error messages for each invalid scenario:
  - "End date cannot be before start date"
  - "Future dates are not allowed"
  - "Date range is too old/extensive"
- Date picker shows visual indicators of invalid selections
- "Show Results" button is disabled or shows validation error with invalid dates
- User cannot proceed with invalid date range configurations
- System provides helpful guidance on valid date range selection
- Error messages are clear and actionable

## Cleanup:
- No cleanup required as report should not be created with invalid date ranges