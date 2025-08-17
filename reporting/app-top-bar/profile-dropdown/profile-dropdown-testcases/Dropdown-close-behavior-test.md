**Title:** Verify profile dropdown close behavior and interaction patterns

**Pre-conditions:**
* User is logged in as an authenticated user

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Dashboard page in the application.
3. Click on the profile avatar button to open the dropdown.
4. Verify the dropdown opens and displays all menu options.
5. Click outside the dropdown area (on page content).
6. Verify the dropdown closes automatically.
7. Reopen the dropdown by clicking the profile avatar.
8. Press the Escape key while dropdown is open.
9. Verify the dropdown closes when Escape is pressed.
10. Reopen the dropdown and click on any menu item.
11. Verify the dropdown closes after menu item selection.
12. Test clicking the profile avatar again while dropdown is open.
13. Verify this toggles the dropdown closed.

**Expected Result:**
* Dropdown opens immediately when profile avatar is clicked
* Clicking outside the dropdown area closes it automatically
* Escape key closes the dropdown from any focused element within
* Selecting any menu item closes the dropdown automatically
* Clicking the profile avatar while dropdown is open toggles it closed
* Dropdown close behavior is consistent across all methods
* No visual glitches or delays during open/close transitions
* Focus management works properly when dropdown closes
* Dropdown doesn't close when clicking inside the dropdown area
* Close behavior works consistently across different screen sizes
* Animation/transition effects (if any) are smooth and professional