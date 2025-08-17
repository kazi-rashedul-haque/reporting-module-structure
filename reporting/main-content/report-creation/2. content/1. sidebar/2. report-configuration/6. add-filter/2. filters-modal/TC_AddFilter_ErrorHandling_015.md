# TC_AddFilter_ErrorHandling_015

## Title:
Verify proper error handling and validation for invalid filter configurations

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open

## Test Steps:
1. Attempt to apply filter without selecting left operand:
   - Leave left operand as "Select"
   - Try to click Apply button
2. Attempt to apply filter with missing right operand:
   - Select left operand (e.g., Campaign)
   - Leave right operand empty
   - Try to click Apply button
3. Test with invalid date ranges:
   - Select date-based left operand (e.g., Campaign Start Date)
   - Enter invalid date format
   - Try to apply filter
4. Test with special characters in text fields:
   - Select text-based operand
   - Enter HTML tags, scripts, special characters
   - Verify input sanitization
5. Test edge cases:
   - Very long text inputs
   - Numeric overflow values
   - Empty spaces as input
6. Test network error scenarios (if applicable)

## Expected Results:
1. Incomplete filter validation:
   - Apply button remains disabled when required fields are missing
   - Clear visual indicators show which fields are required
   - Error messages guide user to complete missing fields
2. Missing left operand:
   - Apply button disabled
   - Error message: "Please select a filter field"
   - User cannot proceed without selection
3. Missing right operand (for operators that require values):
   - Apply button disabled for operators requiring values (Equals, Contains, etc.)
   - Apply button enabled for operators not requiring values (Defined, Not defined)
   - Error message: "Please enter a filter value"
4. Invalid date inputs:
   - Date picker validation prevents invalid dates
   - Clear error messages for invalid date formats
   - Date fields show expected format (MM/DD/YYYY, etc.)
5. Text input validation:
   - HTML tags are stripped or escaped
   - Script injection attempts are blocked
   - Special characters handled appropriately
   - Maximum length limits enforced with character counters
6. Input sanitization:
   - No XSS vulnerabilities
   - SQL injection protection
   - Proper encoding of special characters
7. Error message characteristics:
   - Clear, actionable error messages
   - Error messages appear near relevant fields
   - Errors are announced to screen readers
   - Error styling is visually distinct
8. Recovery from errors:
   - Users can easily correct validation errors
   - Error states clear when inputs are corrected
   - No persistent error states after correction
9. Network error handling:
   - Graceful handling of server errors
   - Retry mechanisms where appropriate
   - User-friendly error messages for technical failures
10. Form remains usable after errors:
    - No form corruption after validation errors
    - All functionality remains accessible
    - Performance not degraded by error states