**Title:** Verify Next button is  not disabled with empty report name.

**Test Steps:**
1. Login to the Workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Leave the Report Name field empty.
5. Optionally enter a description "Test description".
6. Attempt to click the Next button.
7. Verify the button state and system response.
8. Verify any error message that appears.

**Expected Result:**
The Next button should  not be disabled when the report name field is empty or should show a validation error when clicked, an error message should clearly indicate that the report name is required, the user should not be able to proceed to the next step, and the description field value should not affect the validation requirement for the report name.