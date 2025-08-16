**Title:** Verify Remove from Favorites functionality from Actions dropdown

**Pre-conditions:**
* User is on the report details page
* Report is currently in the user's favorites list
* Actions dropdown is accessible

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Open a report that is currently in favorites (star icon is filled).
4. Click on the Actions dropdown button in the report header.
5. Locate the "Remove from Favorites" button with filled star icon.
6. Verify tooltip displays "Remove from Favorites" when hovering over the button.
7. Click on the "Remove from Favorites" button.
8. Verify the star icon changes to outlined state immediately.
9. Verify tooltip changes to "Add to Favorites".
10. Navigate back to the Reports page.
11. Verify the report now displays an outlined star icon in the favorites column.

**Expected Result:**
* Remove from Favorites button is visible in Actions dropdown for favorite reports
* Button displays filled star icon indicating report is a favorite
* Tooltip shows "Remove from Favorites" when hovering over the button
* Clicking the button successfully removes report from favorites list
* Star icon changes to outlined state immediately after clicking
* Tooltip updates to "Add to Favorites" after removing from favorites
* Changes are reflected consistently across report details and reports table views
* Favorite status change persists when navigating between pages