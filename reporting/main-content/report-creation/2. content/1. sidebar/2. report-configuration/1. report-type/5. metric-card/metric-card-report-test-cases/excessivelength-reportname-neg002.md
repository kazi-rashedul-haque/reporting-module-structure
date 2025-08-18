# NEG_ExcessiveLength_ReportName_002

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
    - Report Name: "This_is_an_extremely_long_report_name_that_exceeds_the_maximum_allowed_limit_of_one_hundred_and_twenty_characters_and_should_be_rejected_by_the_system_validation_logic_for_being_too_long_to_handle_properly" (150+ characters)
    - Description: Negative test case for report name exceeding 120 character limit
11. Verify character count indicator shows excess (e.g., "150/120")
12. Click on "Next" button
13. Verify system behavior when report name exceeds maximum length
14. Observe validation messages or input restrictions
15. Check if system truncates input or prevents submission

## Expected Results:
- System prevents input beyond 120 characters OR
- System shows validation error for excessive length
- Character count indicator shows "120/120" when limit is reached
- Input field stops accepting characters after 120 OR
- Clear validation error message appears about length limit
- "Next" button is disabled or shows validation error
- User cannot proceed with report name exceeding maximum length
- System provides clear feedback about character limit violation

## Cleanup:
- No cleanup required as report should not be created with invalid name length