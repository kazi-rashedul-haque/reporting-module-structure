**Title:** Verify handling of duplicate dashboard names during rename

**Preconditions:**
  1. At least two user-created dashboards with different names exist in the Dashboards table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Dashboard List page.
  3. Note the names of existing dashboards in the table.
  4. Click on the "More Actions" button (three dots) for one dashboard.
  5. Click on "Rename" from the dropdown menu.
  6. Enter a dashboard name that already exists for another dashboard.
  7. Attempt to save the changes.
  8. Verify the system's response to duplicate names.

**Expected Result:**
* Block saving duplicate names with an appropriate error message, or allow duplicate names if the business logic permits it
* Display a clear validation message if duplicates are not allowed (e.g., "A dashboard with this name already exists")
* Keep the modal open until a unique name is provided
* Provide specific and actionable error messages for the user