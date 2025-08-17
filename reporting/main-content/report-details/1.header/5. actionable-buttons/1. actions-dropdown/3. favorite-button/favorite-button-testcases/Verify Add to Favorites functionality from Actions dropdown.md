**Title:** Verify Add to Favorites functionality from Actions dropdown

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Open a report that is not currently in favorites (star icon is outlined).
4. Click on the Actions dropdown button in the report header.
5. Locate the "Add to Favorites" button with outlined star icon.
6. Verify tooltip displays "Add to Favorites" when hovering over the button.
7. Click on the "Add to Favorites" button.
8. Verify the star icon changes to filled state immediately.
10. Navigate back to the Reports page.
11. Verify the report now displays a filled star icon in the favorites column.

**Expected Result:**
* Add to Favorites button is visible in Actions dropdown for non-favorite reports
* Button displays outlined star icon indicating report is not a favorite
* Clicking the button successfully adds report to favorites list
* Star icon changes to filled state immediately after clicking
* Changes are reflected consistently across report details and reports table views
* Favorite status persists when navigating between report list and report details pages