**Title:** Verify successful dashboard rename functionality

**Preconditions:**
  1. At least one user-created dashboard exists in the Dashboards table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Dashboard List page.
  3. Note the current name and description of a dashboard.
  4. Click on the "More Actions" button (three dots) for the dashboard.
  5. Click on "Rename" from the dropdown menu.
  6. Enter a new valid dashboard name (1-120 characters, no HTML).
  7. Enter a new valid description (0-240 characters, no HTML).
  8. Click "Save changes" button.
  9. Verify the modal closes and changes are reflected in the table.

**Expected Result:**
* Modal closes successfully after clicking "Save changes"
* Dashboard table reflects the new name and description
* Success notification may appear confirming the rename operation