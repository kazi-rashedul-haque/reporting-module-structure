**Title:** Verify Add to Favorites action functionality

**Pre-conditions:**
* User is logged in as an authenticated user with reporting access
* Report is NOT currently in favorites (no star icon visible in header)

**Test Steps:**
1. Navigate to the "Reporting" application
2. Open an existing report that is not favorited for editing
3. Click on the "Actions" button to open the dropdown menu
4. Verify "Add to Favorites" option is displayed
5. Click on "Add to Favorites" option
6. Verify the report is added to favorites

**Expected Results:**
* "Add to Favorites" option is displayed and clickable
* Clicking the option adds the report to favorites
* Star icon appears next to the report name in the header
* Actions dropdown now shows "Remove from Favorites" option