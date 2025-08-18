**Title:** Verify minimum valid input with single character description.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter a valid report name "Test Report".
5. Click on the Description field.
6. Enter a single character "A".
7. Verify the character counter shows "1/240".
8. Click the Next button to proceed.
9. Verify successful validation occurs.
10. Test with a single number "1".
11. Test with a single special character "@".

**Expected Result:**
Single character input should be accepted as valid input for the description field, the character counter should display "1/240", the Next button should remain enabled, the user should be able to proceed to the next step, and no error messages should be displayed for any valid single character including letters, numbers, and special characters in the description field.