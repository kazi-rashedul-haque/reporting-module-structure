# Title: Ideas_NoXAxisSelected_029

# Pre-Condition: User has access to Reporting app with proper permissions

# Test Steps:
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
    - Report Name: NEG_NoXAxisSelected_029
    - Description: Negative test for attempting to show results without selecting any X-axis value in horizontal bar chart
11. Click on "Next" to create the report
12. Select "Horizontal Bar" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Leave "X Axis" dropdown unselected (no value chosen)
16. Select "Quarterly" from the "Y Axis" dropdown
17. Attempt to click on "Show Results" button
18. Verify that validation error appears for missing X-axis selection
19. Verify "Show Results" button is disabled or validation prevents action
20. Verify appropriate error message indicates X-axis selection is required
21. Verify required field indicator appears for X-axis field
22. Test that chart configuration is incomplete without X-axis
23. Verify system prevents report generation with incomplete configuration

# Expected Results:
- System prevents showing results when no X-axis value is selected
- Validation error message appears indicating X-axis selection is required
- "Show Results" button is disabled or validation prevents action when X-axis is empty
- Error message clearly states "X-axis selection is required" or similar validation message
- Required field indicator (*) appears next to X-axis dropdown
- User cannot proceed with report generation without selecting X-axis value
- System enforces required field validation consistently
- Form validation prevents submission until X-axis is selected
- No chart or data is generated with incomplete configuration
- User remains on configuration with clear error indication
- Red styling or error indicators appear for the required but empty field
- Chart preview area may show placeholder or empty state
- System maintains data integrity by requiring all essential fields
- Configuration is marked as incomplete until X-axis is selected
- No incomplete or invalid reports are created in the system

# Cleanup:
1. Select a valid X-axis value to clear validation error
2. Click "Cancel" button to close the Create Report dialog
3. Verify that no incomplete report is created in the system