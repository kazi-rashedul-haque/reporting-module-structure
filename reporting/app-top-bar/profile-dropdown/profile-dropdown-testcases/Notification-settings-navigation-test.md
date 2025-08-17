**Title:** Verify Notification Settings link navigation to settings page

**Pre-conditions:**
* User is logged in as an authenticated user

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Dashboard page in the application.
3. Click on the profile avatar button to open the dropdown.
4. Locate the "Notification Settings" option in the dropdown menu.
5. Verify the Notification Settings option displays with an appropriate icon.
6. Click on the "Notification Settings" link.
7. Verify navigation occurs to "/c/member-profile/1/settings/notification".
8. Check that the notification settings page loads correctly.
9. Verify the page displays notification preference options.
10. Navigate back to test the link functionality again.

**Expected Result:**
* Notification Settings option is clearly visible in the dropdown menu
* Notification Settings option displays with appropriate icon (typically bell or settings gear)
* Link is properly styled and clickable
* Clicking Notification Settings navigates to "/c/member-profile/1/settings/notification"
* Notification settings page loads successfully within the same tab
* Page displays notification preferences and configuration options
* User can view and modify notification settings as expected
* Navigation maintains user's authenticated session
* Link hover state provides appropriate visual feedback
* Settings page is functional and accessible