**Title:** Verify Show Results button remains disabled after successful report generation

**Pre-conditions:**
* At least one report exists in the report list
* Report configuration has been modified to enable the Show Results button
* Show Results button has been clicked and report generation completed successfully

**Test Steps:**
1. Login to the workspace as an authenticated user.
1. Navigate to the Reporting page.
2. Select any existing report from the Reports table to open the report details page.
3. Make a configuration change(Change the X Axis value) to enable the "Show Results" button.
4. Click the enabled "Show Results" button.
5. Wait for the report generation process to complete successfully.
7. Observe the current state of the "Show Results" button after successful report generation.
8. Attempt to click the "Show Results" button again without making any new configuration changes.

**Expected Result:**
* After successful report generation, the "Show Results" button should return to a disabled state.
* The button should be visually greyed out and non-interactive.
* The disabled state should persist until new configuration changes are made.
* Clicking the disabled button should not trigger any action or additional report generation.