# NEG_ExcessiveLength_Description_003

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
    - Report Name: NEG_ExcessiveLength_Description_003
    - Description: "This is an extremely long description that exceeds the maximum allowed limit of two hundred and forty characters. It should be rejected by the system validation logic for being too long to handle properly. This description is intentionally made very long to test the boundary validation and should trigger an appropriate error message when the user attempts to save or proceed with this report creation process." (350+ characters)
11. Verify character count indicator shows excess (e.g., "350/240")
12. Click on "Next" button
13. Verify system behavior when description exceeds maximum length
14. Observe validation messages or input restrictions
15. Check if system truncates input or prevents submission

## Expected Results:
- System prevents input beyond 240 characters OR
- System shows validation error for excessive description length
- Character count indicator shows "240/240" when limit is reached
- Input field stops accepting characters after 240 OR
- Clear validation error message appears about description length limit
- "Next" button is disabled or shows validation error
- User cannot proceed with description exceeding maximum length
- System provides clear feedback about character limit violation

## Cleanup:
- No cleanup required as report should not be created with invalid description length