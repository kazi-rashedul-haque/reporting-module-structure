# Title: Ideas_ExceedDescriptionLimit_027

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
    - Report Name: NEG_ExceedDescriptionLimit_027
    - Description: Negative test for exceeding description character limit of 240 characters with additional text that goes beyond the maximum allowed length testing validation error handling functionality to ensure system properly validates input fields and prevents creation with oversized descriptions that could cause database or display issues
11. Verify character counter shows excess characters (241+/240)
12. Verify validation error appears for exceeding description character limit
13. Attempt to click on "Next" button
14. Verify that validation prevents proceeding with oversized description
15. Verify appropriate error message is displayed indicating character limit exceeded
16. Verify that input field prevents typing beyond 240 characters OR shows validation error

# Expected Results:
- Report creation is prevented when description exceeds 240 characters
- Validation error message appears indicating description character limit exceeded
- Character counter shows 241+/240 or similar indication of excess characters
- "Next" button is disabled or validation prevents proceeding with oversized description
- Error message clearly states character limit exceeded (e.g., "Description must not exceed 240 characters")
- Input field either prevents typing beyond 240 characters or shows clear validation error
- User cannot proceed to report configuration with oversized description
- System enforces description character limit validation consistently
- Form validation prevents submission until description is within limits
- No navigation to report configuration occurs with invalid input
- User remains on the Create Report dialog with clear error indication
- Red styling or error indicators appear for the invalid field
- System maintains data integrity by preventing oversized descriptions

# Cleanup:
1. Reduce description to within 240 character limit to clear validation error
2. Click "Cancel" button to close the Create Report dialog
3. Verify that no incomplete report is created in the system