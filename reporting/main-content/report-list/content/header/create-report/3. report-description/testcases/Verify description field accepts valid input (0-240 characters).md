**Title:** Verify description field accepts valid input (0-240 characters).

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Click on the Description field.
5. Enter a valid description "This is a test report description".
6. Verify the character counter updates correctly.
7. Clear the field and enter text up to exactly 240 characters.
8. Verify the character counter shows "240/240".
9. Clear the field completely to test empty description.
10. Verify empty description is accepted.

**Expected Result:**
The description field should accept all input ranging from 0 to 240 characters, the character counter should update correctly for all input lengths, the field should accept exactly 240 characters without errors, empty descriptions should be valid since the field is optional, and no error messages should be displayed for any valid input length.