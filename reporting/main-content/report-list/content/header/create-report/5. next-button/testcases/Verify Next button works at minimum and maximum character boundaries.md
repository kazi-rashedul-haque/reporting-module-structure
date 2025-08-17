**Title:** Verify Next button works at minimum and maximum character boundaries.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter minimum report name "A" (1 character) and leave description empty.
5. Click Next and verify successful progression.
6. Return and test with maximum report name (120 characters) and empty description.
7. Click Next and verify successful progression.
8. Return and test with valid report name and maximum description (240 characters).
9. Click Next and verify successful progression.
10. Return and test with maximum length for both fields.
11. Click Next and verify successful progression.

**Expected Result:**
The Next button should work correctly at all valid character boundaries, users should successfully proceed to the Report Configuration page in all boundary test cases, all boundary inputs should be accepted without errors, and data should be preserved correctly during navigation for all character limit combinations.