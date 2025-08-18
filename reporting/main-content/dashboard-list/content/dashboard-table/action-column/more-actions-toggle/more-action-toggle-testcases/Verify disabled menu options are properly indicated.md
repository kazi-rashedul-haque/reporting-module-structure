**Title:** Verify disabled menu options are properly indicated.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the dashboard List page.
3. Click on any more actions toggle button to open the menu.
4. Locate the disabled options (Set as Default Dashboard, Add to Favorites, Remove from Favorites,Export to CSV,Export To Excel).
5. Verify they are visually disabled and show "Upcoming" labels.
6. Attempt to click on disabled options.

**Expected Result:**
- Disabled options should display "Upcoming" labels to indicate future availability.
- Disabled options should not be clickable or should show no response when clicked.
- Hover states should not be applied to disabled options.