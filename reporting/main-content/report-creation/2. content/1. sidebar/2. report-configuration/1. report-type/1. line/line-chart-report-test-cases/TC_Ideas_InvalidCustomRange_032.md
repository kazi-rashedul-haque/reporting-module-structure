# Title: Ideas_InvalidCustomRange_032

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
    - Report Name: NEG_Ideas_InvalidCustomRange_032
    - Description: Negative test for Custom Range with end date before start date validation
11. Click on "Next" to create the report
12. Select "Line" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Custom Range" from the "Time Frame" dropdown
15. Verify date picker appears with "Start Date" and "End Date"
16. Set Start Date to current date
17. Set End Date to a date before the start date (e.g., 7 days ago)
18. Select "Quarterly" from the "X Axis" dropdown
19. Select "# of Ideas Submitted" from the "Y Axis" dropdown
20. Attempt to click on "Show Results" button
21. Verify that validation error appears for invalid date range
22. Verify that "Show Results" button is disabled or validation prevents proceeding
23. Verify appropriate error message is displayed indicating invalid date range

# Expected Results:
- Report creation is prevented when end date is before start date
- Validation error message appears indicating invalid date range
- Error message clearly states "End date must be after start date" or similar validation message
- "Show Results" button is disabled or non-functional with invalid date range
- User cannot proceed to generate results without valid date range
- Date picker may show visual indication of invalid selection (red highlighting, error styling)
- All other configuration fields (Report Type, Data Category, X-axis, Y-axis) remain properly configured
- Form validation prevents chart generation until valid date range is selected
- No chart or table is displayed without proper date range configuration
- User remains on the report configuration screen
- System maintains the current configuration state while showing validation error
- Custom Range validation works correctly to ensure data integrity

# Cleanup:
1. Correct the date range by setting end date after start date
2. Navigate back to Reports list without saving
3. Verify that no incomplete report is created in the system