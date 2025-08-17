**Title:** Verify profile dropdown opens and displays all menu options correctly

**Pre-conditions:**
* User is logged in as an authenticated user

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Dashboard page in the application.
3. Locate the profile avatar button in the top navigation bar.
4. Click on the profile avatar button.
5. Verify the dropdown menu opens below the avatar.
6. Check that all expected menu items are present:
   - Profile link with avatar, name, and username
   - Help option with icon
   - New Features option with icon
   - Notification Settings option with icon
   - Display as Member button with icon
   - Edit Mode button with icon
   - Dark Mode toggle with icon and switch
   - Logout link with icon (should appear in red)
7. Verify each menu item has the appropriate icon.
8. Click outside the dropdown to close it.

**Expected Result:**
* Profile dropdown opens immediately when avatar is clicked
* Profile link displays user avatar, "Super user" name, and "@superuser" username
* Help option is present with appropriate icon
* New Features option is present with appropriate icon
* Notification Settings option is present with appropriate icon
* Display as Member button is present with appropriate icon
* Edit Mode button is present with appropriate icon
* Dark Mode section shows toggle switch with icon and label
* Logout option appears in red color with appropriate icon
* All menu items are properly aligned and styled
* Dropdown closes when clicking outside the menu area
* Menu options are arranged in logical order as specified