**Title:** Verify Next button proceeds with valid report name and optional description.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter a valid report name "Test Report".
5. Optionally enter a description "This is a test report".
6. Click the Next button.
7. Verify the user is navigated to the Report details page.
7. Verify the entered report name is preserved.
8. Verify the description is preserved if it was entered.

**Expected Result:**
The Next button should be enabled , the user should successfully proceed to the Report details page, all entered data including both report name and description should be present in the Report details page, and no error messages should be displayed. The report name should be correctly displayed in the Report details page header.