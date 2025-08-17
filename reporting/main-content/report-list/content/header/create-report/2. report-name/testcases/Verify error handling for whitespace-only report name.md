**Title:** Verify error handling for whitespace-only report name.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Click on the Report Name field.
5. Enter only spaces "   " in the Report Name field.
6. Attempt to click the Next button.
7. Verify validation behavior appears.
8. Clear the field and enter only tabs "\t\t".
9. Attempt to click the Next button again.
10. Verify validation behavior for tabs.

**Expected Result:**
The system should treat whitespace-only input as invalid, display an appropriate error message indicating the report name is required, disable the Next button or show validation error, and prevent the user from proceeding to the next step with whitespace-only input.