**Title:** Verify minimum valid input with single character report name.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Click on the Report Name field.
5. Enter a single character "A".
6. Verify the character counter shows "1/120".
7. Click the Next button to proceed.
8. Verify successful validation occurs.
9. Test with a single number "1".
10. Test with a single special character "@".

**Expected Result:**
Single character input should be accepted as valid input, the character counter should display "1/120", the Next button should be enabled, the user should be able to proceed to the next step, and no error messages should be displayed for any valid single character including letters, numbers, and special characters.