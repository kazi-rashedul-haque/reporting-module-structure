**Title:** Verify empty description field is accepted as valid.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter a valid report name "Test Report".
5. Leave the Description field completely empty.
6. Verify the character counter shows "0/240".
7. Click the Next button to proceed.
8. Verify successful validation occurs.

**Expected Result:**
Empty description should be accepted as valid input since the description field is optional, the character counter should display "0/240", the Next button should remain enabled with valid report name and empty description, the user should be able to proceed to the next step without any issues, and no error messages should be displayed for the empty description field.