**Title:** Verify Save changes button prevents multiple rapid submissions

**Pre-conditions:**
* At least one user report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing user report from the Reports table to open the report details page.
4. Make changes to the report configuration(X axis value changes from the dropdown)
5. The "Save changes" button is enabled.
6. Again click on the "Save changes" button.

**Expected Result:**
* The "Save changes" button should become disabled immediately after the first click.
* Save changes button first click a alert should be displayed
* The rapid clicks should not trigger additional save operations.
