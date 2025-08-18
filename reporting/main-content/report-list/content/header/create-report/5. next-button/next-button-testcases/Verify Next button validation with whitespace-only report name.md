**Title:** Verify Next button validation with whitespace-only report name.

**Test Steps:**
1. Login to the Workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter only whitespace characters "   " in the Report Name field.
5. Enter a valid description "Valid description".
6. Attempt to click the Next button.

**Expected Result:**
The Next button should be disabled or show validation error when the report name contains only whitespace characters, an error message should indicate that a valid report name is required, the user should not be able to proceed to the next step, and the system should treat whitespace-only input as invalid regardless of whether spaces or tabs are used.