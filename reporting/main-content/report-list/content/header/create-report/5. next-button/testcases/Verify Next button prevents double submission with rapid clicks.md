**Title:** Verify Next button prevents double submission with rapid clicks.

**Test Steps:**
1. Login to the Workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter a valid report name "Test Report".
5. Enter a valid description "Test description".
6. Quickly click the Next button multiple times in rapid succession.
7. Verify only one submission is processed.
8. Verify user is navigated to Report Details page.

**Expected Result:**
Only one submission should be processed despite multiple rapid clicks
on the Next button, the user should be navigated to the Report Details page, and no duplicate reports should be created.