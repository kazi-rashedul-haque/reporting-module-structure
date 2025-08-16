# Title: Ideas_ExceedReportNameLimit_026

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
    - Report Name: NEG_Very_Long_Report_Name_That_Exceeds_Maximum_Character_Limit_Of_120_Characters_Testing_Validation_Error_Handling_Extra_Text
    - Description: Negative test for exceeding report name character limit (121+ characters)
11. Verify character counter shows excess characters (121+/120)
12. Verify validation error appears for exceeding character limit
13. Attempt to click on "Next" button
14. Verify that validation prevents proceeding with oversized report name
15. Verify appropriate error message is displayed indicating character limit exceeded
16. Verify that input field prevents typing beyond 120 characters OR shows validation error

# Expected Results:
- Report creation is prevented when report name exceeds 120 characters
- Validation error message appears indicating character limit exceeded
- Character counter shows 121+/120 or similar indication of excess characters
- "Next" button is disabled or validation prevents proceeding with oversized name
- Error message clearly states character limit exceeded (e.g., "Report name must not exceed 120 characters")
- Input field either prevents typing beyond 120 characters or shows clear validation error
- User cannot proceed to report configuration with oversized report name
- System enforces character limit validation consistently
- Form validation prevents submission until report name is within limits
- No navigation to report configuration occurs with invalid input
- User remains on the Create Report dialog with clear error indication
- Red styling or error indicators appear for the invalid field

# Cleanup:
1. Reduce report name to within 120 character limit to clear validation error
2. Click "Cancel" button to close the Create Report dialog
3. Verify that no incomplete report is created in the system