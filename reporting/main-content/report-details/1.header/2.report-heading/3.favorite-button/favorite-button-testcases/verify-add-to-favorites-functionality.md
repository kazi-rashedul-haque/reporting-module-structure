**Title:** Verify Add to Favorites functionality from report details page

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Identify a report that has an empty star icon (indicating it is not favorited).
4. Click on the report title to open the report details page.
5. Verify the favorite button displays an empty star icon with tooltip "Add to Favorites".
6. Click on the "Add to Favorites" button.
7. Verify the button immediately changes to a filled star icon.
8. Verify the tooltip changes to "Remove from Favorites".
9. Navigate back to the Reports page.
10. Verify the report now displays a filled star icon in the favorites column.

**Expected Result:**
* The report is successfully added to the user's favorites list
* The tooltip updates from "Add to Favorites" to "Remove from Favorites"
* The change is reflected consistently across both report details and reports table views
* The favorite status persists when navigating between pages