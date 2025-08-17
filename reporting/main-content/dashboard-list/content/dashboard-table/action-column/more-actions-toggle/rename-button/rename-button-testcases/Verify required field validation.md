**Title:** Verify required field validation for dashboard name

**Preconditions:**
  1. At least one user-created dashboard exists in the Dashboards table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Dashboard List page.
  3. Click on the "More Actions" button (three dots) for any dashboard.
  4. Click on "Rename" from the dropdown menu.
  5. Clear the "Dashboard Name" field completely.
  6. Attempt to click the "Save changes" button.
  7. Verify validation behavior.


**Expected Result:**
* Prevent saving when the dashboard name field is empty
* Display appropriate error message indicating the field is required
* "Save changes" button remains disabled or shows validation feedback
* Asterisk (*) indicator visible next to the Dashboard Name field label
* Modal remains open until a valid name is entered