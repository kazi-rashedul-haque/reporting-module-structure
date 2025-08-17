**Title:** Verify conditional display of Invite Members option

**Pre-conditions:**
* User is logged in as an authenticated user with admin privileges
* Access to workspace settings to toggle invite members feature

**Test Steps:**
1. Login to the workspace as an authenticated user with admin privileges.
2. Navigate to workspace settings or admin panel.
3. Locate the "Invite Members" feature toggle/setting.
4. Ensure the invite members feature is disabled.
5. Navigate to Dashboard page in the application.
6. Click on the profile avatar button to open the dropdown.
7. Verify that "Invite Members" option is NOT present in the dropdown.
8. Close the dropdown and navigate back to workspace settings.
9. Enable the "Invite Members" feature toggle.
10. Return to Dashboard page in the application.
11. Click on the profile avatar button to open the dropdown.
12. Verify that "Invite Members" option IS now present in the dropdown.
13. Test the invite members functionality if present.

**Expected Result:**
* When invite members feature is disabled:
  - "Invite Members" option does not appear in profile dropdown
  - Dropdown displays all other options normally
  - No broken layout or spacing issues in dropdown
* When invite members feature is enabled:
  - "Invite Members" option appears in profile dropdown
  - Option displays with appropriate icon
  - Option is positioned logically within the menu structure
  - Clicking the option functions as expected (opens invite dialog or page)
* Feature toggle works immediately without requiring page refresh
* Conditional display doesn't affect other dropdown functionality
* Setting persists across user sessions