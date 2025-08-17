**Title:** Verify character limit validation for dashboard name and description fields

**Preconditions:**
  1. At least one user-created dashboard exists in the Dashboards table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Dashboard List page.
  3. Click on the "More Actions" button (three dots) for any dashboard.
  4. Click on "Rename" from the dropdown menu.
  5. Enter exactly 121 characters in the "Dashboard Name" field.
  6. Enter exactly 241 characters in the "Description" field.
  7. Attempt to save the changes.
  8. Test with exactly 120 characters in name field and 240 in description.

**Expected Result:**
* Entering more than 120 characters in the dashboard name field
* Entering more than 240 characters in the description field
* Display appropriate validation messages when limits are exceeded
* Allow entering exactly 120 characters in the name field and save successfully
* Allow entering exactly 240 characters in the description field and save successfully
* Display character count indicators to guide the user