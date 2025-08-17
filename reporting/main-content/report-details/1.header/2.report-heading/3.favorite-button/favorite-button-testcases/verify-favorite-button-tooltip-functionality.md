**Title:** Verify favorite button tooltip functionality on report details page

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select a report that is not favorited (empty star icon).
4. Click on the report title to open the report details page.
5. Hover over the favorite button (empty star icon).
6. Verify the tooltip displays "Add to Favorites".
7. Click elsewhere to dismiss the tooltip.
8. Navigate back to the Reports page.
9. Select a report that is favorited (filled star icon).
10. Click on the report title to open the report details page.
11. Hover over the favorite button (filled star icon).
12. Verify the tooltip displays "Remove from Favorites".
13. Click elsewhere to dismiss the tooltip.

**Expected Result:**
* Tooltip appears when hovering over the favorite button
* Tooltip displays "Add to Favorites" when report is not favorited (empty star)
* Tooltip displays "Remove from Favorites" when report is favorited (filled star)
* Tooltip text accurately reflects the current state and available action
* Tooltip appears consistently and is readable
* Tooltip disappears when moving cursor away from the button