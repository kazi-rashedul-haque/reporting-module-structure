**Title:** Verify Help link opens external help documentation

**Pre-conditions:**
* User is logged in as an authenticated user
* Internet connection is available

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Dashboard page in the application.
3. Click on the profile avatar button to open the dropdown.
4. Locate the "Help" option in the dropdown menu.
5. Verify the Help option displays with an appropriate icon.
6. Click on the "Help" link.
7. Verify navigation occurs to "https://help.ideascale.com".
8. Check that the help documentation page loads successfully.
9. Verify the link opens in a new tab/window. [Limited support in Playwright - use manual verification or check target attribute]
10. Return to the original tab and test the link again.

**Expected Result:**
* Help option is clearly visible in the dropdown menu
* Help option displays with appropriate help/question mark icon
* Link is properly styled and clickable
* Clicking Help navigates to "https://help.ideascale.com"
* External help site loads successfully
* Link opens in new tab/window to preserve user's current session
* Help documentation is accessible and functional
* Link hover state provides appropriate visual feedback
* No broken links or 404 errors occur when accessing help