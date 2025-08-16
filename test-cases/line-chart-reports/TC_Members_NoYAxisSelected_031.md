# Title: Members_NoYAxisSelected_031

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
    - Report Name: NEG_Members_NoYAxisSelected_031
    - Description: Negative test for attempting to create report without selecting Y-axis value
11. Click on "Next" to create the report
12. Select "Line" as the "Report Type"
13. Select "Members" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "X Axis" dropdown
16. DO NOT select any value from the "Y Axis" dropdown (leave it empty/unselected)
17. Attempt to click on "Show Results" button
18. Verify that validation error appears for missing Y-axis selection
19. Verify that "Show Results" button is disabled or validation prevents proceeding
20. Verify appropriate error message is displayed indicating Y-axis selection is required

# Expected Results:
- Report creation is prevented when no Y-axis value is selected
- Validation error message appears indicating that Y-axis selection is required
- "Show Results" button is disabled or non-functional when Y-axis is not selected
- Error message clearly states "Y-axis selection is required" or similar validation message
- User cannot proceed to generate results without selecting a Y-axis value
- All other configuration fields (Report Type, Data Category, Time Frame, X-axis) remain properly configured
- Form validation prevents chart generation until Y-axis is selected
- No chart or table is displayed without proper Y-axis configuration
- User remains on the report configuration screen
- System maintains the current configuration state while showing validation error

# Cleanup:
1. Select a valid Y-axis value to clear the validation error
2. Navigate back to Reports list without saving
3. Verify that no incomplete report is created in the system