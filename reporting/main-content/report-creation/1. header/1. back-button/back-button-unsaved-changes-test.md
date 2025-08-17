**Title:** Verify back button triggers unsaved changes warning modal

**Pre-conditions:**
* User is logged in as an authenticated user with reporting access

**Test Steps:**
1. Navigate to the "Reporting" application
2. Open an existing report for editing
3. Make changes to the report configuration
4. Click on the back button in the header
5. Verify that the unsaved changes warning modal appears
6. Click "Continue Editing" button and verify modal closes
7. Make changes again and click back button
8. Click "Discard Changes" button and verify navigation to "Reports" list page

**Expected Results:**
* Unsaved changes warning modal appears when back button is clicked with unsaved changes
* "Continue Editing" button closes modal and keeps user on current page
* "Discard Changes" button closes modal and navigates to "Reports" list page