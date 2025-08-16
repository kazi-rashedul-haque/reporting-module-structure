**Title:** Verify character limit enforcement for description exceeding 240 characters.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Click on the Description field.
5. Enter or paste text containing 241 or more characters.
6. Observe system behavior for truncation, error message, or input prevention.
7. Verify the character counter display shows appropriate values.
8. Attempt to proceed with the Next button if the text was accepted.

**Expected Result:**
The system should prevent input beyond 240 characters, truncate input to exactly 240 characters, or display an error message when the limit is exceeded. The character counter should never exceed "240/240" and if an error occurs, an appropriate error message should be displayed to inform the user of the character limit violation.