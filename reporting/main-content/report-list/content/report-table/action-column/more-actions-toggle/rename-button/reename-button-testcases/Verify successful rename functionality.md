**Title:** Verify successful report rename functionality

**Preconditions:**
  1. At least one user-created report exists in the Reports table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Note the current name and description of a report.
  4. Click on the "More Actions" button (three dots) for the report.
  5. Click on "Rename" from the dropdown menu.
  6. Enter a new valid report name (1-120 characters, no HTML).
  7. Enter a new valid description (0-240 characters, no HTML).
  8. Click "Save changes" button.
  9. Verify the modal closes and changes are reflected in the table.

**Expected Result:**
* Modal closes successfully after clicking "Save changes"
* Report table  reflects the new name and description
* Success notification may appear confirming the rename operation