**Title:** Verify character limit enforcement for report name exceeding 120 characters.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Click on the Report Name field.
5. Enter or paste text containing 121 or more characters.
6. Observe system behavior for truncation, error message, or input prevention.
7. Verify the character counter display shows appropriate values.
8. Attempt to submit the form if the text was accepted.

**Expected Result:**
The system should prevent input beyond 120 characters, truncate input to exactly 120 characters, or display an error message when the limit is exceeded. The character counter should never exceed "120/120" and if an error occurs, the user should not be able to proceed to the next step.