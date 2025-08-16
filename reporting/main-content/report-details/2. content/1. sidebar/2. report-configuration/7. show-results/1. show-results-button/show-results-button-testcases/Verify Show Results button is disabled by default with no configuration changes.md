**Title:** Verify Show Results button is disabled by default with no configuration changes

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Observe the initial state of the "Show Results" button in the Customization sidebar.
5. Verify the button displays the disabled attribute.
6. Attempt to click the disabled "Show Results" button.
7. Verify no action occurs when clicking the disabled button.

**Expected Result:**
* The "Show Results" button should be visually disabled 
* The button should be greyed out and non-interactive.
* Clicking the disabled button should not trigger any action, validation errors, or report generation.
* The button should remain disabled until configuration changes are made to enable it.