**Title:** Verify that clicking the Rename button opens the Rename Report modal

**Preconditions:**
  1. At least one user-created report exists in the Reports table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Locate a user-created report row in the reports table.
  4. Click on the "More Actions" button (three dots) for the report.
  5. Click on "Rename" from the dropdown menu.
  6. Verify the modal appears on screen.
  7. Check all modal elements are present and visible.


**Expected Result:**
* "Rename Report" modal opens successfully
* Modal displays the title "Rename Report" in the header
* "Report Name*" textbox visible with placeholder text "Enter name"
* "Description" textarea visible with placeholder text "Write description"
* Asterisk (*) indicator shows the report name field is required
* "Cancel" button present and clickable at the bottom
* "Save changes" button present at the bottom
* Close button (X) visible in the top right corner of the modal
* Modal overlay appears behind the modal dialog