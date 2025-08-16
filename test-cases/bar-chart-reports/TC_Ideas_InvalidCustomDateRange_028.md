# Title: Ideas_InvalidCustomDateRange_028

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
    - Report Name: NEG_InvalidCustomDateRange_028
    - Description: Negative test for invalid custom date range validation - end date before start date
11. Click on "Next" to create the report
12. Select "Bar" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Custom Range" from the "Time Frame" dropdown
15. Verify date picker appears with "Start Date" and "End Date" fields
16. Set Start Date to today's date
17. Set End Date to 30 days ago (invalid: end date before start date)
18. Select "Quarterly" from the "X Axis" dropdown
19. Select "# of Ideas Submitted" from the "Y Axis" dropdown
20. Attempt to click on "Show Results" button
21. Verify that validation error appears for invalid date range
22. Verify appropriate error message indicates end date must be after start date
23. Test additional invalid scenarios:
    - Future start and end dates
    - Same start and end date
    - Very old dates (>5 years ago)
24. Verify each invalid scenario shows appropriate validation

# Expected Results:
- System prevents showing results with invalid date ranges
- Validation error message appears when end date is before start date
- Error message clearly states "End date must be after start date" or similar
- "Show Results" button is disabled or validation prevents action with invalid dates
- Additional invalid scenarios are properly validated:
  - Future dates: "Dates cannot be in the future"
  - Same dates: "End date must be different from start date"
  - Very old dates: "Date range too old" or similar validation
- User cannot proceed with report generation using invalid date ranges
- System enforces date range validation consistently
- Form validation prevents submission until valid date range is provided
- No chart or data is generated with invalid date inputs
- User remains on configuration with clear error indication
- Red styling or error indicators appear for invalid date fields
- Date picker may prevent selection of invalid dates where applicable
- System maintains data integrity by validating date ranges

# Cleanup:
1. Set valid date range (start date before end date, both in past)
2. Click "Cancel" button to close the Create Report dialog
3. Verify that no incomplete report is created in the system