**Title:** Verify Logout functionality and styling

**Pre-conditions:**
* User is logged in as an authenticated user

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Dashboard page in the application.
3. Click on the profile avatar button to open the dropdown.
4. Locate the "Logout" option at the bottom of the dropdown menu.
5. Verify the Logout option displays with an appropriate icon.
6. Confirm the Logout option appears in red color as specified.
7. Click on the "Logout" link.
8. Verify navigation occurs to the logout URL.
9. Confirm the user is successfully logged out.
10. Verify redirection to appropriate login or home page.
11. Attempt to access a protected page to confirm logout.
12. Test that browser back button doesn't restore authenticated session.

**Expected Result:**
* Logout option is clearly visible at the bottom of the dropdown menu
* Logout option displays in red color to indicate destructive action
* Logout option includes appropriate icon (typically door or exit icon)
* Link is properly styled with red text/background
* Clicking Logout navigates to "https://w1.t1.ideascale.dev/a/workspace/logout"
* User session is completely terminated
* User is redirected to login page or public home page
* All authentication cookies/tokens are cleared
* Attempting to access protected pages redirects to login
* Browser back button doesn't restore authenticated session
* Logout process completes without errors
* Red styling makes logout option clearly distinguishable from other menu items