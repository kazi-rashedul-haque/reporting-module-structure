**Title:** Verify Next button proceeds with valid report name and optional description.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter a valid report name "Test Report".
5. Optionally enter a description "This is a test report".
6. Click the Next button.
7. Verify navigation to the Report Configuration page occurs.
8. Verify the entered report name is preserved.
9. Verify the description is preserved if it was entered.

**Expected Result:**
The Next button should be enabled when a valid report name is entered, the user should successfully proceed to the Report Configuration page, all entered data including both report name and description should be preserved during navigation, and no error messages should be displayed during the transition.