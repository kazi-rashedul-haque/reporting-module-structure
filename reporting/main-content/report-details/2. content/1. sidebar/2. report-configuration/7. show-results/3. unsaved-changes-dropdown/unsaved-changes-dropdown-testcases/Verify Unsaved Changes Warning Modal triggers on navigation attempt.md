**Title:** Verify Unsaved Changes Warning Modal triggers on navigation attempt

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Modify the report configuration (e.g., changing report type, axis, or dataset).
5. Click the "Show Results" button to generate the report with the modified configuration.
5. Do not Click on the save changes button.
6. Attempt to navigate away from the report page (e.g., using the back button).
7. Verify the "Unsaved Changes Warning Modal" appears.

**Expected Result:**
* The "Unsaved Changes Warning Modal" should be triggered when the user attempts to navigate away from the report page without saving recent changes.
* The modal should appear before navigation occurs.