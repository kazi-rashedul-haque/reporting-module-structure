**Title:** Verify error handling for empty report name field.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Leave the Report Name field empty.
5. Attempt to click the Next button.
6. Verify error message or validation behavior appears.

**Expected Result:**
The Next button should be disabled or show a validation error when the report name field is empty, an error message should clearly indicate that the report name is required, and the user should not be able to proceed to the next step without entering a valid report name.