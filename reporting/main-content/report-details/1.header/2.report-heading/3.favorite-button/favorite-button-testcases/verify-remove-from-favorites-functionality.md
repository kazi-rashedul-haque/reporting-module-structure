**Title:** Verify Remove from Favorites functionality from report details page

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Identify a report that has a filled star icon (indicating it is favorited).
4. Click on the report title to open the report details page.
5. Verify the favorite button displays a filled star icon with tooltip "Remove from Favorites".
6. Click on the "Remove from Favorites" button.
7. Verify the button immediately changes to an empty star icon.
8. Verify the tooltip changes to "Add to Favorites".
9. Navigate back to the Reports page.
10. Verify the report now displays an empty star icon in the favorites column.

**Expected Result:**
* The report is successfully removed from the user's favorites list
* The favorite button immediately toggles from filled star to empty star icon
* The tooltip updates from "Remove from Favorites" to "Add to Favorites"
* The change is reflected consistently across both report details and reports table views
* The unfavorited status persists when navigating between pages