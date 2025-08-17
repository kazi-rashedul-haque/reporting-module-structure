**Title:** Verify rename modal pre-fills with current dashboard name and description

**Preconditions:**
  1. At least one user-created dashboard with name and description exists in the Dashboards table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Dashboard List page.
  3. Locate a dashboard with an existing name and description.
  4. Note the current dashboard name and description values.
  5. Click on the "More Actions" button (three dots) for the dashboard.
  6. Click on "Rename" from the dropdown menu.
  7. Verify the modal opens and check field values.

**Expected Result:**
• Rename modal opens with the "Dashboard Name" field pre-filled with the current dashboard name
• "Description" field pre-filled with the current description (if any)
• Description field displays empty with placeholder text visible if no description exists
• Both fields are editable and ready for modification