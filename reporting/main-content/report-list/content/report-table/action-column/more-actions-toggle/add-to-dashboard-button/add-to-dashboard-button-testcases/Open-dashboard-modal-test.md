**Title:** Verify that clicking the Add to Dashboard button opens the Add to Dashboard modal

**Preconditions:**
  1. At least one report exists in the Reports table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Locate a report row in the reports table.
  4. Click on the "More Actions" button (three dots) for any report.
  5. Click on "Add to Dashboard" from the dropdown menu.
  6. Verify the modal appears on screen.
  7. Check all modal elements are present and visible.

**Expected Result:**
  The "Add to Dashboard" modal opens successfully, modal displays the title "Add to Dashboard" in the header, search textbox is visible with placeholder text "Search", "No options to show" message displays initially in the results area, "Cancel" button is present and clickable at the bottom, "Add to Dashboard" button is present but disabled by default, close button (X) is visible in the top right corner of the modal, modal overlay appears behind the modal dialog.