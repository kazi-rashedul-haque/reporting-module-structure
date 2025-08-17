**Title:** Verify Remove from Favorites action functionality

**Pre-conditions:**
* User is logged in as an authenticated user with reporting access
* Report is currently in favorites (star icon visible in header)

**Test Steps:**
1. Navigate to the "Reporting" application
2. Open an existing report that is already favorited for editing
3. Click on the "Actions" button to open the dropdown menu
4. Verify "Remove from Favorites" option is displayed
5. Click on "Remove from Favorites" option
6. Verify the report is removed from favorites

**Expected Results:**
* "Remove from Favorites" option is displayed and clickable
* Clicking the option removes the report from favorites
* Star icon disappears from next to the report name in the header
* Actions dropdown now shows "Add to Favorites" option