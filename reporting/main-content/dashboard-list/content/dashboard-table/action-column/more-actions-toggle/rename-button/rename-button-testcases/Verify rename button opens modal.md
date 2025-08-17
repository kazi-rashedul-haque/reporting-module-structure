**Title:** Verify that clicking the Rename button opens the Rename Dashboard modal

**Preconditions:**
  1. At least one user-created dashboard exists in the Dashboards table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Dashboard List page.
  3. Locate a user-created dashboard row in the dashboards table.
  4. Click on the "More Actions" button (three dots) for the dashboard.
  5. Click on "Rename" from the dropdown menu.
  6. Verify the modal appears on screen.
  7. Check all modal elements are present and visible.


**Expected Result:**
* "Rename Dashboard" modal opens successfully
* Modal displays the title "Rename Dashboard" in the header
* "Dashboard Name*" textbox visible with placeholder text "Enter name"
* "Description" textarea visible with placeholder text "Write description"
* Asterisk (*) indicator shows the dashboard name field is required
* "Cancel" button present and clickable at the bottom
* "Save changes" button present at the bottom
* Close button (X) visible in the top right corner of the modal
* Modal overlay appears behind the modal dialog