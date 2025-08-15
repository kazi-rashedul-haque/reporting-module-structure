**Title:** Verify rename modal close functionality and cancel behavior

**Preconditions:**
  1. At least one user-created report exists in the Reports table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Click on the "More Actions" button (three dots) for any report.
  4. Click on "Rename" from the dropdown menu.
  5. Make changes to the report name and/or description fields.
  6. Test each close method:
     - Click the "Cancel" button
     - Click the close button (X) in the top right corner
     - Press the Escape key
  7. Verify the modal behavior for each method.


**Expected Result:**
* All close methods successfully close the modal without saving changes
* Any modifications made to the fields are discarded
* Original report name and description remain unchanged in the table
* No validation errors occur when closing
* Modal completely disappears from the screen