**Title:** Verify special character handling in report name field.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Click on the Report Name field.
5. Enter various special characters "@#$%&*+=!?".
6. Verify field acceptance or rejection behavior.
7. Test common punctuation marks ".,;:'-".
8. Test unicode characters "àáâãäåæçèé".
9. Attempt to proceed with the Next button.
10. Verify validation behavior for each character type.

**Expected Result:**
The system should consistently accept or reject special characters with clear rules, display appropriate error messages if characters are rejected, allow the user to proceed if characters are accepted, and maintain consistent behavior across all different types of special characters and unicode characters.