**Title:** Verify Show Results button behavior with incomplete configuration

**Pre-conditions:**
* At least one report exists in the report list
* The sidebar is currently expanded
* Donut chart radio button is selected

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Select Donut chart from the Report Type options.
5. Leave some required configuration fields empty or unselected.
6. Locate the Show Results button.
7. Click on the Show Results button.
8. Verify appropriate validation messages appear for incomplete fields.
9. Complete the missing configuration fields.
10. Click Show Results again and verify the chart displays properly.

**Expected Result:**
* Show Results button should be visible when configuration is incomplete
* Clicking with incomplete configuration should show validation messages
* Validation messages should clearly indicate which fields are required
* Completing configuration should allow successful chart generation