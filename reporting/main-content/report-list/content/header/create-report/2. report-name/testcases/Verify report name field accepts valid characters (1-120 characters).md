**Title:** Verify report name field accepts valid characters (1-120 characters).

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Click on the Report Name field.
5. Enter a valid report name "Test Report".
6. Verify the character counter updates correctly.
7. Clear the field and enter text up to exactly 120 characters.
8. Verify the character counter shows "120/120".

**Expected Result:**
The report name field should accept all valid input between 1 and 120 characters, the character counter should update correctly for all inputs, the field should accept exactly 120 characters without any errors, and no error messages should be displayed for valid input lengths.