**Title:** Verify Actions dropdown navigation and accessibility.

**Preconditions:**
* User is on a report details page
* Actions dropdown contains multiple menu items

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Reporting page and open any report details.
3. Locate the "Actions" button in the report header.
4. Click the "Actions" button to open the dropdown menu.
5. Verify dropdown menu opens and displays all available actions:
   - Add to Dashboard
   - Export to CSV (if available)
   - Export to Excel (if available)
   - Rename
   - Schedule Email Report (if available)
   - Add to Favorites
   - Clone
   - Delete
6. Verify "Add to Dashboard" is the first item in the menu.
7. Click outside the dropdown to close it.
8. Test keyboard navigation: Tab to Actions button, press Enter.
9. Use arrow keys to navigate through menu items.
10. Press Enter on "Add to Dashboard" menu item.
11. Verify modal opens correctly.

**Expected Result:**
* Actions dropdown opens when clicked
* All menu items are displayed correctly
* "Add to Dashboard" is accessible and clickable
* Keyboard navigation works properly
* Menu items are properly organized and labeled
* Disabled items are clearly indicated
* Modal opens when "Add to Dashboard" is selected