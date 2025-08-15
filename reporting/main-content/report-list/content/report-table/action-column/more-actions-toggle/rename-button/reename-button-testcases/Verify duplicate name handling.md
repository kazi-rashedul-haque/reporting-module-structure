**Title:** Verify handling of duplicate report names during rename

**Preconditions:**
  1. At least two user-created reports with different names exist in the Reports table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Note the names of existing reports in the table.
  4. Click on the "More Actions" button (three dots) for one report.
  5. Click on "Rename" from the dropdown menu.
  6. Enter a report name that already exists for another report.
  7. Attempt to save the changes.
  8. Verify the system's response to duplicate names.

**Expected Result:**
* Block saving duplicate names with an appropriate error message, or allow duplicate names if the business logic permits it
* Display a clear validation message if duplicates are not allowed (e.g., "A report with this name already exists")
* Keep the modal open until a unique name is provided
* Provide specific and actionable error messages for the user