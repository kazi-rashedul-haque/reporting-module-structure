**Title:** Verify Show Results button prevents multiple rapid submissions

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
1. Navigate to the Reporting page.
2. Select any existing report from the Reports table to open the report details page.
3. Make a configuration change(X Axis dropdown change to another value)
4. Verify the "Show Results" button is initially enabled
4. Rapidly click the "Show Results" button multiple times in quick succession (double-click or triple-click).
5. Observe the button behavior during rapid clicking.
8. Wait for the single report generation to complete.
9. Verify the final button state after completion.

**Expected Result:**
* Only the first click on the "Show Results" button should trigger report generation.
* The button should immediately become disabled after the first click to prevent double-clicking.
* The button should remain in loading state until the single report generation completes.
* No error states or duplicate processing should occur due to rapid clicking.